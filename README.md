# Entity In The Dark

A presentation to introduce **Identification Schemes and Entity Authentication** for the course [CS60065: Cryptography and Network Security](https://monosijm.github.io/CNS-2025.html). Our team consisted of 
- [BerserkWInter](https://github.com/BerserkWInter)
- [SaiPragnaan](https://github.com/SaiPragnaan)
- [me :)](https://github.com/Majestic9169)

## Contents

1. Identification Schemes
    - What is Identification
    - How do you Identify?
    - Challenge-Response
1. Private Key Identification
    - MAC based and Parallel Session Attacks
    - Identity-bound MAC based
    - Proving Security and Intruder-in-the-Middle Attacks
1. Mutual Authentication
    - 3-way Authentication and Reflection Attacks
    - Secure Mutual Authentication
1. References

## Setting Up Marp and Viewing the Presentation

This presentation was made using [Marp](https://marpit.marp.app/). To setup a presentation like this simply use the [marp-cli public template](https://github.com/yhatt/marp-cli-example)

1. The template provides a workflow to upload your presentation to github pages. You can view our presentation [here](https://majestic9169.github.io/entity-in-the-dark/)

> [!CAUTION] 
> Make sure to set `Settings -> Pages -> Source` to **Github Actions** in your repo to prevent Github from adding their default pages workflow

2. To build and view locally just run 

```bash
npm run build
```

This will create a  `public/` directory inside which you can start an http-server, e.g.

```bash
# php inbuilt
php -S 0.0.0.0:8080
# python inbuilt
python -m http.server 8080
# node module
npm install http-server -g
http-server -p 8080
```

3. The starter template also recommends installing the Marp VSCode extension which will let you preview your presentation in VSCode with `Ctrl+Shift+V`

## References

- [Cryptography Academy](https://cryptographyacademy.com/identification-schemes/)
- [Challenge-Response Authentication](https://en.wikipedia.org/wiki/Challenge%E2%80%93response_authentication)
- [Parallel Session Attacks](https://link.springer.com/content/pdf/10.1007/978-3-540-85257-5_24.pdf?pdf=inline+link)
- [Authentication in SSH](https://web.archive.org/web/20041014002830/http://www.cag.lcs.mit.edu/~rugina/ssh-procedures/)

---

i would like to add public key authentication eventually too, but that's for when i have for too much free time
