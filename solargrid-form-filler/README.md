
# SolarGrid Term Generator 🚀

Sistema web em Flask para **gerar contratos personalizados (Word `.docx`) automaticamente**, com base em um modelo de contrato enviado pelo usuário.

---

## 📌 Funcionalidades:

- ✅ Upload de modelo de contrato `.docx`
- ✅ Preenchimento automático dos campos (Nome, CPF, CNPJ, UC, Percentual de Desconto, Representante, etc.)
- ✅ Geração de contratos para **Pessoa Física** e **Pessoa Jurídica**
- ✅ Substituição automática de placeholders no Word como:  
`{{NOME}}`, `{{CPF}}`, `{{EMAIL}}`, `{{TELEFONE}}`, `{{CNPJ}}`, `{{UC}}`, `{{DESCONTO}}`, `{{DATA_ATUAL}}`, etc.
- ✅ Sistema de Login simples (usuário e senha fixos)
- ✅ Front-end com layout estilizado (SolarGrid Branding)
- ✅ Download automático do contrato preenchido

---

## 🛠️ Tecnologias usadas:

- Python 3.x
- Flask
- python-docx
- HTML + CSS (puro, com estilo simples e responsivo)

---

## 🗂️ Estrutura de Pastas:

```
SolarGrid-Form-Filler/
├── app.py
├── requirements.txt
├── Procfile (se for deploy)
├── templates/
│   ├── index.html
│   └── login.html
├── static/
│   └── logo.png
├── uploads/
├── output/
└── README.md
```

---

## ✅ Como Rodar Localmente:

1. **Clone o projeto:**

```bash
git clone https://github.com/seuusuario/solargrid-form-filler.git
cd solargrid-form-filler
```

2. **Instale as dependências:**

```bash
pip install -r requirements.txt
```

3. **Execute o Flask:**

```bash
python app.py
```

4. **Abra no navegador:**

```
http://127.0.0.1:5000/
```

---

## ✅ Login padrão:

- **Usuário:** `admin`
- **Senha:** `1234`

*(Você pode mudar isso dentro do `app.py`)*

---

## ✅ Como preparar os modelos de contrato:

Seu Word `.docx` precisa conter os placeholders no formato:

```
{{NOME}}
{{CPF}}
{{EMAIL}}
{{TELEFONE}}
{{CNPJ}}
{{UC}}
{{DESCONTO}}
{{DATA_ATUAL}}
```

👉 O sistema vai substituir automaticamente por tudo que o usuário preencher no formulário.

---

## ✅ Sugestões de melhorias futuras:

- Login com múltiplos usuários
- Geração automática de PDF
- Histórico de contratos gerados
- Deploy na nuvem (Render, Railway, etc.)

---

## ✅ Licença:

Projeto para uso interno SolarGrid ou fins educacionais.  
Sinta-se livre para adaptar e melhorar!
