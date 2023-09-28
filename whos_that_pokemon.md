
# whos_that_pokemon

## starting the challenge with installing the apk into our android device 


```bash
    adb install whos_that_pokemon.apk 
```
when we open the application on the emulator we will find a page with input field and button (GUESS) 
 from the challenge name we can understand that we need to find pokemon name

![Screenshot from 2023-09-29 01-33-10](https://github.com/mohammedatary/UMDCTF2023-mobile/assets/37233306/eaae8ec3-5cc2-42e6-b902-c15a2502dc9d)


I prefer to use jadx or jadx-gui to understand the application 

```bash 
    jadx-gui whos_that_pokemon.apk 
```

now we let's navigate to jadx-gui
we will search for saved strings and it's values 
![image](https://github.com/mohammedatary/UMDCTF2023-mobile/assets/37233306/266d24ba-b9a8-43c5-af4d-1c3734b138ac)

strings mostly saved in res/values/strings.xml 
if we search for pokemon inside it , it will show two results 


first result : ![image](https://github.com/mohammedatary/UMDCTF2023-mobile/assets/37233306/5b57ed22-70e0-4403-a3e0-6a01f52a16b4)

seconed result : ![image](https://github.com/mohammedatary/UMDCTF2023-mobile/assets/37233306/f594b767-3fb1-4e49-9f90-e1321a790697)

wait a minute ! I have a question . did you watch pokemons before ? 

we found that the value of pokemon is ### Terrapulseonic

let's try it 

![image](https://github.com/mohammedatary/UMDCTF2023-mobile/assets/37233306/57952956-a639-4801-b369-bd24ec1d63ae)


Guess what ? 

![image](https://github.com/mohammedatary/UMDCTF2023-mobile/assets/37233306/623eddc0-dfe5-4294-b7a1-9aeca4fa6ad4)



