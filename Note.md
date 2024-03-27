## Implementing fastgan for Data Synthesis








###   Read the official README.MD file also  
first go to stylegan2-ada official github page and read that carefully now follow these steps to implement the stylegan2 ada for data synthesis
1. clone the reposetory 
2. creat a conda environment 
2. read the requiremnt section carefully and install the necessary package as said 
4. prepare the data what you want to train and then use the dataset_tool.py code to prepare it 
5. it is using square data so be careful avout it 
6. now also note some time the extension name is not matching during training so be careful about it and change accordingly like PNG to png so on 
7. use good gpu because it si going to take a long time to trian the model 
8. run this command: python train.py --outdir=~/out/training-runs --data=~/mydataset.zip --gpus=1 ( it will take zip file and that will be created by dataset_tool.py code)
9. now after trianing use this code: python generate.py --outdir=out1 --trunc=0.7 --seeds=6600-6625 –network=/home/akbar/stylegan2-ada-pytorch/~/training-runs/00000-Kiranfarm_15m_altitude-auto1/network-snapshot-025000.pkl (it is my code os u can change accoding to you )
10. now compare the data 
###