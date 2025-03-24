
# LabElasticSearch - Grupo 07

Este repositório contém o notebook e as configurações necessárias para executar buscas léxica, semântica, híbrida e criativa utilizando Elasticsearch.

## COMO EXECUTAR

### 1. Clone o repositório

```bash
git clone https://github.com/paolamoura/LabElasticSearch-Group07.git
cd LabElasticSearch-Group07
```

### 2. Crie o ambiente virtual

```bash
python3.12 -m venv venv
```

### 3. Ative o ambiente virtual

- No **Linux/macOS**:
```bash
source venv/bin/activate
```

- No **Windows**:
```bash
venv\Scripts\activate
```

### 4. Instale as dependências

```bash
pip install -r requirements.txt
```

### 5. Atualize o arquivo de dependências (opcional)

```bash
pip freeze > requirements.txt
```

### 6. Suba os containers com o Elasticsearch + Kibana

```bash
docker-compose up -d
```

### 7. Inicie o Jupyter Notebook

```bash
jupyter notebook
```

Acesse o notebook pelo link exibido no terminal, geralmente: [http://localhost:8888](http://localhost:8888)

## GRUPO

- Paola Kathrein Moura Marques
- João Henrique Almeida Xavier
- Victor Vinicius Freire de Araujo
- Marcos Antônio Cardoso Pereira
- Samuel Cabral de Luna