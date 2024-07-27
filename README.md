# Sistema de Amortização de Empréstimos

## Descrição
Este programa em C++ calcula a tabela de amortização de um empréstimo utilizando o sistema Price. Ele solicita ao usuário o valor inicial do empréstimo, a taxa de juros e o período de tempo (em meses), e exibe a tabela de amortização detalhada.

## Compilação e Execução

### Compilação
Para compilar o programa, utilize um compilador C++. Aqui está um exemplo usando g++:
sh
g++ -o amortizacao amortizacao.cpp
Execução
Após a compilação, execute o programa com:

sh
Copiar código
./amortizacao
Uso
Ao iniciar o programa, insira o valor inicial do empréstimo.
Em seguida, insira a taxa de juros (em porcentagem).
Por fim, insira o período de tempo do empréstimo (em meses).
O programa exibirá a tabela de amortização, mostrando:

Parcela
Prestação
Juros
Amortização
Saldo Devedor
Exemplo de Saída
yaml
Copiar código
Parcela | Prestação | Juros | Amortização | Saldo Devedor
----------------------------------------------------------
  1     | 903.46    | 150.00| 753.46      | 9246.54 
  2     | 903.46    | 138.70| 764.76      | 8481.78 
  3     | 903.46    | 127.23| 776.23      | 7705.55 
  4     | 903.46    | 115.58| 787.88      | 6917.67 
  5     | 903.46    | 103.77| 799.69      | 6117.97 
  6     | 903.46    | 91.77 | 811.69      | 5306.28 
  7     | 903.46    | 79.59 | 823.87      | 4482.41 
  8     | 903.46    | 67.24 | 836.22      | 3646.19 
  9     | 903.46    | 54.69 | 848.77      | 2797.42 
 10     | 903.46    | 41.96 | 861.50      | 1935.92 
 11     | 903.46    | 29.04 | 874.42      | 1061.49 
 12     | 903.46    | 15.92 | 887.54      | 0.00
Estrutura do Código
O código está organizado em funções para facilitar a manutenção e a leitura:

trivia(): Limpa o buffer de entrada.
inserirPeriodo(): Solicita o período de tempo ao usuário.
inserirJuros(): Solicita a taxa de juros ao usuário.
inserirValor(): Solicita o valor inicial do empréstimo ao usuário.
f4(float v, float j, int p): Calcula e exibe a tabela de amortização.
f1(): Função principal que coleta os dados do usuário e inicia o cálculo.
main(): Configura a localidade para Português e chama a função f1().
