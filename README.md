- 👋 Hi, I’m @EveraldoFern
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
EveraldoFern/EveraldoFern is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->
# importando o SQLite
import sqlite3 as lite


# Criando conexão
con = lite.connect('dados.db')

# Criando tabela
with con:
    cur = con.cursor()
    cur.execute("CREATE TABLE Inventario(id INTEGER PRIMARY KEY AUTOINCREMENT,nome TEXT, local TEXT, descricao TEXT,marca TEXT,  data_da_compra DATE, valor_da_compra DECIMAL, serie TEXT, imagem TEXT)")

