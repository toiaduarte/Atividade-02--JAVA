# Atividade-02--JAVA

package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio02 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite um número inteiro: ");
        int numero = leitor.nextInt();

        // IFS INDEPENDENTES
        if (numero > 0) {
            System.out.println("É positivo.");
        }
        if (numero % 2 == 0) {
            System.out.println("É par.");
        }
        if (numero % 5 == 0) {
            System.out.println("É múltiplo de 5.");
        }
        
        // Módulo do número para verificar dois dígitos (entre 10 e 99)
        int modulo = Math.abs(numero);
        if (modulo >= 10 && modulo <= 99) {
            System.out.println("Tem dois dígitos.");
        }

        leitor.close();
    }
}

package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio02 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite um número inteiro: ");
        int numero = leitor.nextInt();

        // IFS INDEPENDENTES
        if (numero > 0) {
            System.out.println("É positivo.");
        }
        if (numero % 2 == 0) {
            System.out.println("É par.");
        }
        if (numero % 5 == 0) {
            System.out.println("É múltiplo de 5.");
        }
        
        // Módulo do número para verificar dois dígitos (entre 10 e 99)
        int modulo = Math.abs(numero);
        if (modulo >= 10 && modulo <= 99) {
            System.out.println("Tem dois dígitos.");
        }

        leitor.close();
    }
}

package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio03 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite a temperatura em Celsius: ");
        double temp = leitor.nextDouble();

        System.out.print("Digite a umidade relativa do ar (%): ");
        double umidade = leitor.nextDouble();

        // IFS INDEPENDENTES
        if (temp >= 38) {
            System.out.println("Alerta de calor extremo!");
        }
        if (umidade < 30) {
            System.out.println("Alerta de umidade baixa!");
        }
        if (temp >= 35 && umidade < 20) {
            System.out.println("Alerta de risco de queimada!");
        }

        leitor.close();
    }
}


package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio04 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite o primeiro número inteiros: ");
        int num1 = leitor.nextInt();

        System.out.print("Digite o segundo número inteiro: ");
        int num2 = leitor.nextInt();

        if (num2 == 0) {
            System.out.println("A verificação não pode ser feita pois o divisor é zero.");
        } else {
            if (num1 % num2 == 0) {
                System.out.println("O primeiro número é múltiplo do segundo.");
            } else {
                System.out.println("O primeiro número NÃO é múltiplo do segundo.");
            }
        }

        leitor.close();
    }
}


package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio05 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite o ano: ");
        int ano = leitor.nextInt();

        if ((ano % 4 == 0 && ano % 100 != 0) || (ano % 400 == 0)) {
            System.out.println("O ano " + ano + " é bissexto.");
        } else {
            System.out.println("O ano " + ano + " NÃO é bissexto.");
        }

        leitor.close();
    }
}



package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio06 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite o valor da compra: R$ ");
        double valorCompra = leitor.nextDouble();

        double frete;
        if (valorCompra >= 199.00) {
            frete = 0.00;
        } else {
            frete = 24.90;
        }

        double total = valorCompra + frete;

        System.out.printf("Valor do frete: R$ %.2f%n", frete);
        System.out.printf("Total a pagar: R$ %.2f%n", total);

        leitor.close();
    }
}


package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio07 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite a hora do dia (0 a 23): ");
        int hora = leitor.nextInt();

        if (hora >= 0 && hora <= 11) {
            System.out.println("Bom dia!");
        } else if (hora >= 12 && hora <= 17) {
            System.out.println("Boa tarde!");
        } else if (hora >= 18 && hora <= 23) {
            System.out.println("Boa noite!");
        } else {
            System.out.println("Hora inválida!");
        }

        leitor.close();
    }
}


package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio08 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite a velocidade máxima da via (km/h): ");
        double velMaxima = leitor.nextDouble();

        System.out.print("Digite a velocidade do veículo (km/h): ");
        double velVeiculo = leitor.nextDouble();

        if (velVeiculo <= velMaxima) {
            System.out.println("Dentro do limite. Não há multa.");
        } else if (velVeiculo <= velMaxima * 1.20) {
            System.out.println("Infração Média.");
        } else if (velVeiculo <= velMaxima * 1.50) {
            System.out.println("Infração Grave.");
        } else {
            System.out.println("Infração Gravíssima.");
        }

        leitor.close();
    }
}



package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio09 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite o salário do funcionário: R$ ");
        double salario = leitor.nextDouble();

        System.out.print("Digite o tempo de casa em anos: ");
        double tempoAnos = leitor.nextDouble();

        double percentual;

        if (tempoAnos < 1) {
            percentual = 0.0;
        } else if (tempoAnos <= 3) {
            percentual = 0.05;
        } else if (tempoAnos <= 10) {
            percentual = 0.10;
        } else {
            percentual = 0.15;
        }

        double valorBonus = salario * percentual;

        System.out.printf("Percentual de bônus: %.0f%%%n", percentual * 100);
        System.out.printf("Valor do bônus: R$ %.2f%n", valorBonus);

        leitor.close();
    }
}


package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio10 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite o nome de usuário: ");
        String usuario = leitor.nextLine();

        // Comparação de texto com equalsIgnoreCase
        if (usuario.equalsIgnoreCase("admin")) {
            System.out.print("Digite a senha: ");
            String senha = leitor.nextLine();

            if (senha.equals("java123")) {
                System.out.println("Acesso liberado.");
            } else {
                System.out.println("Senha incorreta.");
            }
        } else {
            System.out.println("Usuário não encontrado.");
        }

        leitor.close();
    }
}


package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio11 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite a frequência (%): ");
        double frequencia = leitor.nextDouble();

        if (frequencia < 75) {
            System.out.println("Reprovado por falta.");
        } else {
            System.out.print("Digite a média final do aluno: ");
            double media = leitor.nextDouble();

            if (media >= 7.0) {
                System.out.println("Aprovado!");
            } else if (media >= 5.0) {
                System.out.println("Recuperação.");
            } else {
                System.out.println("Reprovado por nota.");
            }
        }

        leitor.close();
    }
}

package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio12 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite o saldo da conta: R$ ");
        double saldo = leitor.nextDouble();

        System.out.print("Digite o limite diário de saque: R$ ");
        double limiteDiario = leitor.nextDouble();

        System.out.print("Digite o valor do saque solicitado: R$ ");
        double valorSaque = leitor.nextDouble();

        if (saldo < valorSaque) {
            System.out.println("Saldo insuficiente.");
        } else {
            if (valorSaque > limiteDiario) {
                System.out.println("Valor ultrapassa o limite diário de saque.");
            } else {
                saldo -= valorSaque;
                System.out.printf("Saque efetuado com sucesso! Novo saldo: R$ %.2f%n", saldo);
            }
        }

        leitor.close();
    }
}

package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio13 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite o primeiro número: ");
        double num1 = leitor.nextDouble();

        System.out.print("Digite o segundo número: ");
        double num2 = leitor.nextDouble();

        System.out.println("Escolha a opção:");
        System.out.println("1 - Soma");
        System.out.println("2 - Subtração");
        System.out.println("3 - Multiplicação");
        System.out.println("4 - Divisão");
        int opcao = leitor.nextInt();

        switch (opcao) {
            case 1 -> System.out.printf("Resultado: %.2f%n", num1 + num2);
            case 2 -> System.out.printf("Resultado: %.2f%n", num1 - num2);
            case 3 -> System.out.printf("Resultado: %.2f%n", num1 * num2);
            case 4 -> {
                if (num2 == 0) {
                    System.out.println("Não é possível dividir por zero!");
                } else {
                    System.out.printf("Resultado: %.2f%n", num1 / num2);
                }
            }
            default -> System.out.println("Opção inválida.");
        }

        leitor.close();
    }
}

package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio14 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite o número do mês (1 a 12): ");
        int mes = leitor.nextInt();

        switch (mes) {
            case 1, 3, 5, 7, 8, 10, 12 -> System.out.println("Este mês possui 31 dias.");
            case 4, 6, 9, 11 -> System.out.println("Este mês possui 30 dias.");
            case 2 -> System.out.println("Este mês possui 28 dias.");
            default -> System.out.println("Mês inválido.");
        }

        leitor.close();
    }
}

package br.com.seunome.lista02;

import java.util.Scanner;

public class Exercicio15 {
    public static void main(String[] args) {
        Scanner leitor = new Scanner(System.in);

        System.out.print("Digite o tipo do veículo (1 - Carro / 2 - Moto): ");
        int tipoVeiculo = leitor.nextInt();

        double tarifaHora = 0;
        boolean tipoValido = true;

        // PARTE 5: SWITCH
        switch (tipoVeiculo) {
            case 1 -> tarifaHora = 8.00;
            case 2 -> tarifaHora = 5.00;
            default -> {
                System.out.println("Opção inválida.");
                tipoValido = false;
            }
        }

        // Apenas continua se o tipo de veículo for válido
        if (tipoValido) {
            System.out.print("Digite a quantidade de horas: ");
            int horas = leitor.nextInt();
            leitor.nextLine(); // Limpa o buffer de memória

            double valorBruto = tarifaHora * horas;

            System.out.print("Possui cupom de desconto? (sim/nao): ");
            String temCupom = leitor.nextLine();

            double valorFinal = valorBruto;

            // PARTE 4: IF ANINHADO
            if (temCupom.equalsIgnoreCase("sim")) {
                if (valorBruto >= 50.00) {
                    valorFinal = valorBruto * 0.80; // 20% de desconto
                } else {
                    System.out.println("O cupom vale apenas para contas acima de R$ 50,00.");
                }
            }

            // PARTE 1: IFS INDEPENDENTES
            if (horas > 12) {
                System.out.println("Aviso: Permanência longa.");
            }
            if (horas > 24) {
                System.out.println("Aviso: Cobrança de diária aplicada.");
            }

            // PARTE 3: ELSE IF (Classificação da permanência)
            if (horas <= 2) {
                System.out.println("Classificação: Permanência curta.");
            } else if (horas <= 6) {
                System.out.println("Classificação: Permanência média.");
            } else {
                System.out.println("Classificação: Permanência longa.");
            }

            System.out.printf("Valor final a pagar: R$ %.2f%n", valorFinal);
        }

        leitor.close();
    }
}
