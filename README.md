# AI - case study - Project Ask questions for multiple pdf documents

Para criar o token_api do hugginface ir no site
https://huggingface.co/settings/tokens

Para executar a aplicação usar o comando:
streamlit run app.py

/**\*\***PYVENV**\***/
Para instalar o Python 3.9 usar o comando:
sudo apt update
sudo apt install python3.9

Para criar o ambiente virtual usar o comando:
python3.9 -m venv nome_do_seu_ambiente_virtual
por ex: python3.9 -m venv venv

Para ativar o ambiente virtual do python usar o comando:
source nome_do_seu_ambiente_virtual/bin/activate
por ex: source venv/bin/activate

Para desativar o ambiente virtual:
deactivate

/**\*\***REQUIREMENTS.TXT**\***/
Para instalar as dependencias a partir de um requirements.txt existente usar o comando:
pip install -r requirements.txt

Para atualizar as dependências para as versões mais recentes, você pode usar o comando:
pip install --upgrade -r requirements.txt

Para gerar o arquivo requirements.txt com as dependencias instaladas no ambiente virtual usar o comando:
pip freeze > requirements.txt
