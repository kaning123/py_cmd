# pycmd_command
It is a simple python program to create commands and use it. 
The operation method is as follows:
## 1.Create command (example:-a):
        
        try:
            from pycmd_command import command
        except ImportError:
            print('unable to find pycmd_command')
        example=command('a',1)
        
## 2.Find out if the command was exist:
        
        print(example.command_exist()[0])
        
### Enter the following at the Command Prompt:
        
        python test.py 
        
### The output is as follows:
        
        False
## 3.Delete the command
  ```
   example.delete_command()
   print(example.command_exist()[0])
  ```
### The output is as follows:
```
Traceback (most recent call last):
  File "c:\Users\.py", line 2, in <module>
    print(example.command_exist()[0])
AttributeError: 'command' object has no attribute 'command_exist'
```
## 4.Run command
```
example.run_command(yourfunc)


   
