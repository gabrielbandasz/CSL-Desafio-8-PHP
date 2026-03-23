# 🍪 Desafio 8 – Cookies e Sessions no PHP

## 📖 Introdução

Para entender por que precisamos de **Cookies** e **Sessions**, primeiro precisamos entender uma característica do protocolo HTTP:

👉 Ele é **stateless (sem estado)**.

Isso significa que:
- Cada requisição é independente
- O servidor **não lembra** quem você é
- Não há "memória" entre páginas

### 🧠 Problema
Sem persistência:
- Você teria que fazer login a cada página
- Carrinhos de compra seriam perdidos
- Preferências não seriam salvas

### ✅ Solução
Utilizamos:
- **Cookies**
- **Sessions**

---

## 🍪 Cookies

São **arquivos pequenos armazenados no navegador do usuário**.

### 📌 Características:
- Armazenados no cliente
- Enviados automaticamente ao servidor
- Ideais para dados simples

### 🧾 Exemplos de uso:
- Tema (claro/escuro)
- Idioma
- "Lembrar usuário"

---

### 🔧 Criar um Cookie
```php
setcookie("nome", "valor", tempo_expiracao, caminho, dominio, seguro, http_only);
