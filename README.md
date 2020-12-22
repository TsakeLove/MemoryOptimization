# MemoryOptimization

### Сode before optimization

```
static void Main(string[] args)
      
      {
            int[,,,] Matrix= new int[10,10,10];
            int res = 0;

	    for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    for (int k = 0; k < 10; k++)
                    {
                        Matrix[k, j, i]+=2;
                    }
                }
            }

            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    for (int k = 0; k < 10; k++)
                    {
                        Matrix[k, j, i]--;
                    }
                }
            }
            

        }
```
### Result
 ![alt text](picture/result_before.png "Code_after")​
### Сode after optimization
 ![alt text](picture/code_after.png "Code_after")​
 ### Result
 ![alt text](picture/result_after.png "Code_after")​

