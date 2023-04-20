# ui_click_launch
# one click launcher of ui for linux .sh
```
cd 
cd /text-generation-webui
python server.py # --model your_model_name --wbits 4 --groupsize 128 --model_type Llama # add any other command line args you want, no extension for name
xdg-open http://127.0.0.1:7860
```

#make file executable <br />
#depends on ur system I right click  on desktop and it allows to create a launcher then I link it to the script <br />
![Capture d’écran du 2023-04-19 13-45-25](https://user-images.githubusercontent.com/39489591/233065462-839d2db7-320d-49f7-b795-0ea4b065749d.png)

#this part starts a dark ui the script is a bit more advanced
```

#!/bin/bash
cd
pwd
source /home/user_name/miniconda3/etc/profile.d/conda.sh
conda activate textgen
#eval "$(conda shell.bash hook)"
#xdg-open http://localhost:7860/?__theme=dark
cd 
cd text-generation-webui 
python server.py # --model your_model_name --wbits 4 --groupsize 128 --model_type Llama # add any other command line args you want


 read -n 1 -s -r -p "Press any key to close."

```
#replace server.py with provided  file to autolaunch it's in darkmode
