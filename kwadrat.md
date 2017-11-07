<h1> To jest program obliczający równanie kwadratowe</h1>
<h2> Wybieramy biblioteki</h2> 

#include <stdio.h>
#include <math.h>
<h2> to jest funkcja główna programu</h2>

int main()
<h2> dane wejsciowe funkcji</h2>
<p>
{
float a,b,c,delta;
printf("podaj wspolczynnik a: ");
scanf("%f",&a);
printf("podaj wspolczynnik b: ");
scanf("%f",&b);
printf("podaj wspolczynnik c: ");
scanf("%f",&c);
</p>


<h3>jeżeli a=0 nie ma funkcji kwadratowej</h3>
if
        (a==0)
        {
        printf("to nie rownanie kwadratowe");
        }
else
<h2>funkcja licząca deltę</h2>
<p>delta =(b*b)-(4*a*c);</p>

<h2> W zależności od obliczonych wartości delty</h2>

<h2> jeśli wartość delty jest większa od 0 ma dwa rozwiązania</h2>
<blockquote>
        {
 
        if
                (delta>0)
                {
		
                printf("pierwsze rozwiazanie x: %2f\n",(-b-sqrt(delta))/(2*a));
                printf("drugie rozwiazanie x: %2f\n",(-b+sqrt(delta))/(2*a));
                }
        else
	{
        
</blockquote>


<h2> jeśli wartość delty jest równa 0 jest jedno rozwiązanie równania </h2>
<blockquote>
		
                        if
                        (delta ==0)
                        {
			printf("jedno rozwiazanie x: %2f\n",-b/(2*a));
                        }
			else
	
</blockquote>

<h2> jeżeli jest delta mniejsza od zera brak rozwiązania równania </h2>
<blockquote>
	{
		if
		(delta < 0)
		{
		printf("brak rozwiazan");
</blockquote>
                }
        }

} 
<h1> Zakończenie programu </h1>
 
return 0;

}
