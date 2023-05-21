Exercice 2 :
![image](https://github.com/ElAm1ne/python_cle_publique_2023/assets/114306633/af88451b-ca43-47f2-8e1e-4505e7cc0724)


Voici les screens de l'execution de l'exercice 1 :
![image](https://github.com/ElAm1ne/python_cle_publique_2023/assets/114306633/7fd825f8-629e-4056-bad1-b2677bd5e334)
![image](https://github.com/ElAm1ne/python_cle_publique_2023/assets/114306633/40f4f6e3-384b-424c-b7a6-5b7a15a95dac)

# python_cpp
Exemple d'utilisation d'un composant en python
Utilise pybind11
apres git clone, faire:
```
cd python_cpp
git submodule init
git submodule update
```

Pour compiler

```
cd hello
make
```

Pour utiliser
```
python3
>>> import hello_component
>>> hello_component.greet()
'hello, world'
>>> hello_component.getVersion()
'1.0'
>>> 
```
## Sujet  Création d'un composant clé permettant le chiffrement asymetrique utilisant la courbe secp256k1
utiliser [micro-ecc](https://github.com/jluuM2/micro-ecc) qui est deja un sous repertoire (git submodule) de composant_cle<br/>
test a realiser:
```
import composant_cle
macle = composant_cle.cle()
macle.initialize(”4b8e29b9b0dddd58a709edba7d6df6c07ebdaf5653e325114bc5318c238f87f0”)
macle.getPrivateKey() -> retourne la valeur d’initialisation
macle.getPublicKey() -> retourne “f2ce1e40befbebaf4045f1a6d126b7b949e7d5adea33f84a09a904093456f4fd504b1f70755be4cef27625b1e6b893e05ffeb361f2971fda1d6be5e730a74303”

