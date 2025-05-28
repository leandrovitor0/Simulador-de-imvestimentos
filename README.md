 Descrição
Esta planilha foi desenvolvida para auxiliar no planejamento financeiro, com foco em investimentos mensais 
e projeções de patrimônio acumulado ao longo dos anos. Ela também calcula dividendos mensais com base no rendimento
da carteira e sugere aportes mensais de acordo com o perfil do investidor.

Funcionalidades
- Configurações iniciais: Definição de salário, rendimento da carteira e sugestão de investimento mensal.
- Projeções de cenários: Estimativa de patrimônio acumulado e dividendos mensais para diferentes períodos (2, 5, 10, 20 e 30 anos).
- Acompanhamento mensal: Registro de aportes reais e cálculo da meta atingida em cada mês.
- Distribuição de investimentos: Percentuais sugeridos para diferentes tipos de fundos imobiliários (FIIs) com base no perfil do investidor.

 Estrutura da Planilha
1. Configurações:
   - Salário: `D15`
   - Rendimento da carteira: `D16`
   - Sugestão de investimento mensal: `D17`
   - Investimento mensal: `D20`
   - Taxa de rendimento mensal: `D22`
   - Patrimônio acumulado: `D23`
   - Dividendos mensais: `D24`

2. Cenários:
   - Projeções de patrimônio e dividendos para diferentes períodos (2 a 30 anos) na tabela de `A27:D31`.

3. Acompanhamento Mensal:
   - Registro de aportes reais e cálculo da meta atingida na tabela de `B37:D49`.

4. Distribuição de FIIs:
   - Percentuais sugeridos e valores calculados para diferentes tipos de FIIs na tabela de `B52:D58`.

 Fórmulas Utilizadas
- Cálculo de patrimônio acumulado:
  ```excel-{ "functionLanguage": "en-US", "argSeparator": ",", "numberDecimalSeparator": "." }
  =FV(taxa_mensal,qtd_anos*12,aporte*-1)
Cálculo de dividendos mensais:
=patrimonio*rendimento_carteira
Percentuais de FIIs:
=procv($C$34&"-"&B52,Planilha2!$A:$D,4,FALSE)
Como Usar
Insira os valores iniciais nas células de configurações.
Verifique as projeções de patrimônio e dividendos na tabela de cenários.
Registre os aportes reais mensalmente na tabela de acompanhamento.
Utilize os percentuais sugeridos para distribuir os investimentos entre os tipos de FIIs.
