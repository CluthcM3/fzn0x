<h1 align="center">I'm Fauzan!</h1>
<h3 align="center"><i>A passionate "formalized javascript" programmer and web developer.</i></h3>
<p align='center'>
  <a href="https://fzn0x.bearblog.dev/"><img height="64" src="https://cdn2.iconfinder.com/data/icons/ios-14-custom-application/62/application-56-256.png"></a>&nbsp;&nbsp;
  <a href="https://discordapp.com/users/780424233343647794"><img height="64" src="https://cdn3.iconfinder.com/data/icons/popular-services-brands-vol-2/512/discord-256.png"></a>&nbsp;&nbsp;   
</p>  

## Currently listening to

<a href="https://volt.fm/fzn0x" target="_blank"><img src="https://my-spotify-badge.vercel.app/api/now-playing.svg" width="540" height="52" alt="now playing"></a>

<details>
  <summary>A "boring" programmer section</summary>
  
## Programming is hard (As an idealist)
Everyone doing programming with their own perspective with no general perspective how to do it. I like to code in any unopinionated and opinionated environments and any programming style my teams would like to use. I could adapt with it. but if asked, I prefer to use a programming style that can separate each utility, library and business logic in folders, and write it in a functional style in a language that allows it to do that (if I can I force to). Nevertheless, I'm not against programming languages and other programming language paradigms that allows the different things.

## The truth way I like to writing functions is
If you don't know anything about [Ramda](https://github.com/ramda/ramda), I would to recommend you to learn it, it is interesting. One that's took my interest is with how they write a function using `R.pipe`.

```js
const f = R.pipe(Math.pow, R.negate, R.inc);

f(3, 4); // -(3^4) + 1
```

Isn't interesting? when you can create a function with something called left-to-right composition (R.pipe definition)?

Since I interest with it, I create a research purpose workspace to do the exact same thing but without the practical functional functions like `R.negate`, `R.inc`, etc. Instead I wrap the built-in prototypes functions to replace those functions and filter it with some magic codes to see the parent object (where it goes), if it's the part of built-in prototypes, then execute it differently from the ones user-defined functions. 

```js
function toLowerCase(value) {
  return value.toLowerCase();
}

let toLowercasedString = h.merge(h.string.toString, h.string.toLowerCase);
console.log(toLowercasedString("GREETINGS FROM HOCUS"));
// or with user-defined function
toLowercasedString = h.merge(h.string.toString, toLowerCase);
console.log(toLowercasedString("INSPIRED BY RAMDA ❤️"));
// fault tolerant
toLowercasedString = h.merge(h.string.toString, toLowerCase, String);
console.log(toLowercasedString("INSPIRED BY RAMDA ❤️"));
toLowercasedString = h.merge(String, h.string.toString, toLowerCase, Object);
console.log(toLowercasedString("INSPIRED BY RAMDA ❤️"));
```

Resulting to:

```sh
greetings from hocus
inspired by ramda ❤️
INSPIRED BY RAMDA ❤️
[String: 'INSPIRED BY RAMDA ❤️']
```

## A "boring" programmer.
Most programmers forcing their way how to do programming, but I prefer not, especially to the point of bothering other people, I'm a boring programmer, the truth is, I only use what I need, I just write code in a formal and described way with a collection of functions and emphaty (mostly to avoid long-term bugs :smile:), that's all. But yes, I can adapt in any programming environment and multidisciplinary teams.
</details>
