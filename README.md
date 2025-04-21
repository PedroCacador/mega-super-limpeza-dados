# 🧹 MegaSuper - Limpeza de Dados

Este repositório contém o processo completo de limpeza de dados do e-commerce fictício **MegaSuper Vendas**, que enfrentava problemas sérios com dados desorganizados, inconsistentes e com diversos erros que comprometeriam análises futuras.

## 📊 Descrição do Projeto

A base de dados original apresenta transações de vendas com:
- Dados faltantes e inconsistentes
- Produtos com nomes despadronizados
- Cálculos incorretos de totais
- Duplicatas
- CEPs e Estados inválidos
- Tipos de dados errados

Este projeto trata, padroniza e valida todas essas informações, deixando o DataFrame pronto para análises mais avançadas.

---

## ⚙️ Tecnologias Utilizadas

- Python 3.10+
- pandas
- numpy
- datetime
- Git e GitHub

---

## 🧪 Etapas de Limpeza Realizadas

1. **Leitura e Renomeação de Colunas**  
   - Leitura do CSV original com encoding `utf-8`
   - Padronização de nomes de colunas para snake_case

2. **Tratamento de Dados Faltantes**
   - Substituição de `NaN` por valores padrão (0, "desconhecido", etc.)
   - Conversão de datas e horas com formatos coerentes

3. **Padronização de Dados**
   - Normalização de textos para lowercase
   - Padronização de nomes de produtos usando expressões regulares
   - Limpeza e formatação de CEPs

4. **Validação e Correção de Dados**
   - Cálculo correto da coluna `Total` com base em `Valor * Quantidade + Frete`
   - Filtros para remover valores absurdos/inválidos

5. **Remoção de Duplicatas**
   - Eliminação de registros repetidos
   - Reset de índices

6. **Geração de Relatório**
   - Impressão no console de um relatório final com estatísticas do processo
---

## 📁 Estrutura do Projeto

