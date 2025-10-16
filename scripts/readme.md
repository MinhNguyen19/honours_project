### Install packages
pip install torch torchvision torchaudio --index-url https://download.pytorch.org/whl/cu121

pip install pyarrow jupyter pandas seaborn accelerate bitsandbytes transformers peft protobuf sentencepiece 

pip install transformers accelerate bitsandbytes sentencepiece huggingface_hub tqdm numpy pandas scikit-learn hf_xet

pip install "huggingface_hub[cli]"

### create & activate env
python -m venv bert_env 
bert_env\Scripts\Activate.ps1

### Connect notebook to virtual machine