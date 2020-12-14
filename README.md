// c++
#include "stdio.h"
main()
{
	int A[10], I, max, jum;
	int total;
	float rata;
	
	printf("Masukan 10 Nilai Mahasiswa\n");
	for(I=0; I<=9; I++)
	{
		printf("Nilai Mahasiswa ke - %i ", (I+1));
		scanf("%i", &A[I]);
		total = total + A[I]; 
	}
	for (I=0; I<=9; I++)
	{
		printf ("%4i", A[I]);
	}
	rata = total / I ;
	jum = 0;
	for (I=0; I<=9; I++)
	{
		if (A[I] < rata)
		{ jum ++;
		}
	 } 
	 printf("\nRata-rata Nilai Mahasiswa : %2.f\n", rata);
	 printf("%i Nilai Mahasiswa Yang di bawah Rata-rata", jum);
	 return 0;
	 
}
