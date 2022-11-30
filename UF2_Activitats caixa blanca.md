# Activitats: 

Per dibuixar els diagrames de flux podeu fer servir [draw.io](https://draw.io) o qualsevol altra eina online.

1. Calcula el CC de les següents figures:
  - ![image](https://user-images.githubusercontent.com/110727546/204613022-4ab64342-2e06-438d-a7e8-570685b3c406.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204613180-6d55bf09-28b8-417e-96f4-f71a762ac44c.png)
  - ![image](https://user-images.githubusercontent.com/110727546/204655229-8c3f28d7-3d8b-4746-a55d-331f89da39d2.png)

  - **Resultat 1:**CC= 16-14+2=4
  - **Resultat 2:**CC=16-14+2=4
  - **Resultat 3:**CC=8-6+2=4


2. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:
  - ![image](https://user-images.githubusercontent.com/110727546/204615125-363e5e6c-173b-4ec0-8c0b-cb97985ade06.png)

  - **Diagrama:**
  
    ![image](https://user-images.githubusercontent.com/113586166/204738210-ff70b880-60ad-4118-b7e0-c1152261ffc7.png)

  - **Resultat:** CC=2+1=3

  

3. Dibuixa el diagrama de flux representat per aquest codi i després calcula la seva CC:

```
public class proves {
    public static  String queEmPoso(int temperatura) {
        String roba = "res";
        if(temperatura<0){
           roba = "roba d'esquiar";
        }
        else if(temperatura<10){
           roba = "roba de muntanya";
        }
        else if(temperatura<20){
           roba = "roba d'hivern";
        }
        else if(temperatura<30){
           roba = "roba d'estiu";
        }
        return roba;
    }    
}
```

  - **Diagrama:**

  ![image](https://user-images.githubusercontent.com/113586166/204743308-364b9ad0-99b6-4ddc-8228-bfeae7ee7930.png)

  - **Resultat:** CC=3+1=4

4. Dibuixa el diagrama de flux representat per aquest codi, calcula la seva CC i crea una prova per a cada camí posible:

```
    public static Boolean llumsEncesos(int hora) {
        Boolean llums = false;
        if(hora <= 8 || hora >= 20){
            llums = true;
        }
        return llums;
    }
```
  - **Diagrama:**

![image](https://user-images.githubusercontent.com/113586166/204744209-fb68385d-111d-42ac-9e6b-601680455033.png)

  - **Resultat:** CC= 2+1= 3 (Hi ha un 2 en el lloc de les condicións ja que dins del IF apareixen dos condicions separades per un OR.)
  - **Resultat proves camins:**
  P1= hora=7 -->llums=true
  P2= hora=21 --> llums=true
  P3= hora=10 --> llums=false

5. Investiga sobre les proves de caixa negra:

  - **Què són?**
  -Les proves de caixa negra, son proves en les que no es necessari coneixer el codi, unicament la funcionalitat del programa.
  Aquestes proves es fan respecte a la funcvionalitat es a dir, comprovem que realment el programa fa la funcio per la qual ha estat desenvolupat.
  Perexemple un programa que ha de sumar A+B jo he de introduir 2+2 i com a resultat m'ha de treure 4.
  La unica funció de les proves de caixa negra es, comprovar que el codi faci el que es demana, no en's interesa com ho fa ni si tot funciona correctament, unicament en's interesa comprovar que dona els resultats correctes.
  - **Quina diferència principal tenen sobre les de caixa blanca?**
  - La diferencia principal es que en aquest cas noconeixem el codi, i en el cas de la caixa blanca si.
  
