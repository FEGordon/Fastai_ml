# Fastai_ml
#how to use paperspace machine for fastai "machine learning for coders" class

#to get started
1. go to fastai directory: `/Users/Hoptoad/fastai`

2. start paperspace machine: `paperspace machines start --machine-id "psvrve5xk"`
You will see {} in terminal window if this works

3. SSH into the paperspace machine:
`ssh -i id_rsa_paperspace paperspace@184.105.188.134`

note: the rsa key is in the "id_rsa_paperspace" file

4. Note: this is optional list everything, fastai, and data files.  May wish to update this periodically.  
see: https://github.com/reshamas/fastai_deeplearn_part1/blob/master/tools/paperspace.md

5. cd into the fastai directory on the paperspace machine

6. Launch Jupyter notebook using this command:
`jupyter notebook --no-browser --port=8889 --NotebookApp.allow_remote_access=True`

7. Open a new terminal window and go to the fastai directory.

8. SSH into the paperspace machine to create a tunnel that redirects
local localhost to the paperspace machine local host (ie create a wormhole)
`ssh -N -L localhost:8889:localhost:8889 paperspace@184.105.188.134 -i id_rsa_paperspace`

9. copy the url with token into the browser


#to shut down
1. close jupyter in browser
2. kill tunnel (use control-c)
3. close jupyer in command line using control-C and then typing "y" into console
4. exit the paperspace machine by typing exit into command prompt.  you will see logout which confirms it's shut
5. Stop paperspace machine: `paperspace machines stop --machine-id psvrve5xk`.  
You will see {} to indicate this happened.





