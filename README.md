while True:
    palavra = input("Digíte 'continue' para provar que você não é um robô:")
    if palavra == 'continue':
        break
    elif palavra != 'continue':
        print("\nSeguindo as orientações anteriores, tente novamente.\n")

nome = str(input("Próximo passo:\n\n\nNome do aluno:"))
materia= str(input("Matéria:"))
print("Olá, {}. Vamos calcular sua média em {}, por favor, digite seus dados abaixo:".format(nome, materia))
try:

 var1 = float(input("Primeira nota de {}:".format(materia)))
 var2 = float(input("Segunda nota de {}:".format(materia)))
 var3 = float(input("Terceira nota de {}:".format(materia)))
 var4 = float(input("Quarta nota de {}:".format(materia)))
 media = float(var1 + var2 + var3 + var4) / 4
 if media >=90:
    print("PARABÉNS!!! Com uma média de {:.1f} você foi aprovado(a) com EXCELÊNCIA em {}, {}!".format(media, materia, nome))
 elif media >=60 <90:
    print("{}, a sua média em {} foi {:.1f} e você foi aprovado(a).\nParabéns!".format(nome, materia, media))
 elif media >=50 <60:
    print("Com a média de {:.1f} você precisará realizar a prova de recuperação.\nMas não se desespere {}, {} é uma matéria fácil, e nós sabemos que basta você estudar que passará. \nBOA SORTE!".format(media, nome, materia))
 else:
    print("Infelizmente você foi reprovado(a) {}. a sua média em {} foi {:.1f}, e infelizmente não foi o suficiente.\nTe esperamos no proximo ano!\n:)".format(nome, materia, media))
except:
    print("O valor informado não é um número.\nPor favor, informe suas notas usando NÚMEROS!")

input()

