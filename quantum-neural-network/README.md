# Setting up environment
## Prerequisites
since numpy>=1.20.0 has bunch of deprecation,<br>
the latest version of qiskit(0.23.5) no more supports numpy<=1.19.5<br>
but in order to use pytorch 1.7.1, we have to set python<3.9<br>
and it forces to use numpy 1.19.5, so we will get error if we run `import qiskit`.

my successful environment was as follows.<br>
(install cuda toolkit 10.2 first!!!)
```
conda create -n qistorch python=3.8
conda activate qistorch

pip install numpy==1.19.5
pip install qiskit==0.23.4
conda install pytorch torchvision torchaudio cudatoolkit=10.2 -c pytorch
```