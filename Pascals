# include <stdio.h>
# include <math.h>

int factorial(int n){
    int product =1;
    for(int i =1; i<=n; i++){
        product *=i;
    }
    return product;
}
    
int choose(int n, int r){
    int answer;
    answer = factorial(n)/(factorial (r) * factorial (n-r));
    return answer;
}

void triangle (int n){
    int row;
    int column;
    for (row =0; row<=n-1;row++) {
        for (column = 1; column <=(3*n-3*row - 3); column++){
            printf(" ");
        }
        for (column =0;column<=row;column++){
            printf("%-6.0d",choose(row,column));

        }
    printf("\n");
    }
}

int main(void) {
  int rows;

  do {
    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    if (rows >= 0) {
      triangle(rows);
    }
  } while (rows >= 0);

  return 0;
}
