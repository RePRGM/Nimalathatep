# Nimalathatep
Nimalathatep is a Nim shellcode payload generation project that aims to get a stealthy binary inro your hands quickly. All methods use well-known API-call sequences.

# Evasion
AV/EDR avoidance is performed through AES encryption followed by Base64, with the payload itself only being decrypted at runtime. The IV is currently static, but I aim to change this in the future. 

# Compilation
Ensure you have NIM downloaded from here: https://nim-lang.org/install.html </br>
</br>
To compile: </br>
```nim -d:release c .\nimalathatep.nim``` </br>
</br>
[<img alt="alt_text" width="1000" src="compilation.PNG" />]
</br>

# Usage
Limited functionality right now, but simply run the executable and pass it the API method and your raw shellcode file: </br> </br>
```.\nimalathatep.exe <apiMethod> <binFile>``` </br>
</br>
[<img alt="alt_text" width="1000" src="payload_creation.PNG" />]
</br>

# Defender Check
[<img alt="alt_text" width="1000" src="full-usage.gif" />]
