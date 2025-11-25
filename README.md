

# 🚀 Desafio DevOps – CI/CD 🛠️

### 🎓 Projeto Final de DevOps – Impacta

---

## 📘 Visão Geral

Esta é uma API REST desenvolvida em **Flask**, criada para demonstrar uma pipeline completa de **CI/CD** utilizando **GitHub Actions** e **Render.com**.

A aplicação só é implantada após passar pelos testes automatizados, garantindo estabilidade e qualidade no deploy.

---

## 📊 Status da Pipeline

| Etapa       | Ferramenta                  | Status       |
| ----------- | --------------------------- | ------------ |
| Build       | GitHub Actions              | 🛠️ OK       |
| Testes (CI) | unittest                    | ✅ Aprovado   |
| Deploy (CD) | Render Deploy Action + Hook | 🚀 Realizado |
| Produção    | Render.com                  | 🌐 Online    |

---

## ⚙️ Tecnologias Usadas

* Python 3.9
* Flask
* Flask-JWT-Extended
* Swagger UI
* unittest
* GitHub Actions
* Render.com

---

## 💡 Fluxo da Pipeline (CI/CD)

1. **Build:** instala dependências e prepara o ambiente
2. **Test:** executa `unittest`
3. **Deploy:** enviado automaticamente ao Render se os testes passarem

---

## 💻 Como Rodar Localmente

```bash
git clone https://github.com/SEU-USUARIO/SEU-REPO.git
cd SEU-REPO
pip install -r requirements.txt
python app.py
```

Acesse em:
👉 [http://127.0.0.1:1313](http://127.0.0.1:1313)

---

## 📚 Endpoints

### **GET /**

Retorna:

```json
{"message":"API is running"}
```

### **GET /items**

```json
{"items":["item1","item2","item3"]}
```

### **GET /login**

Gera token JWT

### **POST /protected** 🔐

Requer header:
`Authorization: Bearer <TOKEN>`

---


## 🧪 Testes Automatizados

Arquivo: `test_app.py`
Testes incluem:

* rota `/`
* login
* proteção JWT
* lista de itens

Executar manualmente:

```bash
python -m unittest discover
```

---

## 🌐 Produção

URL do Render:
👉 **https://desafio-devops-6ern.onrender.com**

---

## 👤 Autor

**Gustavo Bezerra**

