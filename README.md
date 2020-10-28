# Azure-GPU-Setup
1. After logging into the VM, clone the this setup repo:
```
git clone https://github.com/Sheldenshi/Azure-GPU-Setup.git
```
Add execution permission for the setup scripts:
```
chmod +x *.sh
```
if Permission denied, run:
```
sudo -s
```
2. cd into the cloned repo:
```
cd Azure-GPU-Setup
```
3. Run the first setup script:
```
bash gpu-setup-part1.sh
```
Upon completion, the VM will restart automatically. SSH into the VM again.
4. After re-logging into the VM, you can use the following command to show GPU information:
```
nvidia-smi
```
![Image of Yaktocat](https://github.com/Sheldenshi/Azure-GPU-Setup/blob/main/sc1.png)
5. cd into the cloned repo again:
```
cd Azure-GPU-Setup
```
6. Run the second setup script:
```
bash gpu-setup-part2.sh
```
7. Run the following command:
```
python gpu-test.py
```
