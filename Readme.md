# 📑 README.md – Projeto Banco em Pandas

```markdown
# Banco em Pandas 🏦

Um mini-sistema bancário desenvolvido em **Python + Pandas** para o desafio Itaú.  
Permite criar contas, registrar transações (depósitos, saques e transferências) e gerar relatórios em **JSON**.

---

## 🚀 Funcionalidades
- Criar contas de clientes com saldo inicial.
- Registrar transações:
  - Depósitos
  - Saques
  - Transferências entre contas
- Consultar relatórios consolidados de contas e transações.
- Exportar relatórios em formato **JSON**.

---

## 📂 Estrutura do Projeto
```
├── banco.py              # Código principal
├── relatorio_banco.json  # Saída gerada com contas e transações
├── requirements.txt      # Dependências do projeto
└── README.md             # Documentação
```

---

## ⚙️ Instalação

1. Clone este repositório:
   ```bash
   git clone https://github.com/seuusuario/banco-pandas.git
   cd banco-pandas
   ```

2. Crie um ambiente virtual (opcional, mas recomendado):
   ```bash
   python -m venv venv
   source venv/bin/activate   # Linux/Mac
   venv\Scripts\activate      # Windows
   ```

3. Instale as dependências:
   ```bash
   pip install -r requirements.txt
   ```

---

## ▶️ Uso

Execute o script principal:

```bash
python banco.py
```

Isso irá:
- Criar contas iniciais.
- Registrar algumas transações de exemplo.
- Gerar o arquivo `relatorio_banco.json` com os dados consolidados.

---

## 📊 Exemplo de Saída (JSON)

```json
{
  "contas": [
    {"id_cliente": 1, "nome": "Maria", "conta": "001", "saldo": 1050.0},
    {"id_cliente": 2, "nome": "João", "conta": "002", "saldo": 550.0}
  ],
  "transacoes": [
    {"id_transacao": 1, "conta_origem": null, "conta_destino": "001", "tipo": "deposito", "valor": 200, "data": "2025-11-20 18:00:00"},
    {"id_transacao": 2, "conta_origem": "002", "conta_destino": null, "tipo": "saque", "valor": 100, "data": "2025-11-20 18:05:00"},
    {"id_transacao": 3, "conta_origem": "001", "conta_destino": "002", "tipo": "transferencia", "valor": 150, "data": "2025-11-20 18:10:00"}
  ]
}
```

---

## 📌 Requisitos
- Python 3.9+
- Pandas >= 2.0.0

---

## 🔮 Extensões Futuras
- Relatórios filtrados por cliente ou tipo de transação.
- Exportação em CSV/Excel.
- Dashboard com gráficos de movimentação.
- Integração com banco de dados (SQLite/PostgreSQL).

---

## 👨‍💻 Autor
Projeto desenvolvido para o **Desafio Itaú** utilizando **Pandas**.
```

---

