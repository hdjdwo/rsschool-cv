1. Vlad Skaskevich
2. email: vlad.1488skaskevich@gmail.com   tel: +375293217143
3. I am a beginner developer. I came to this course to improve my knowledge in this area, as well as to look at the work of other people and their ways to solve certain problems and get a fair assessment of my knowledge. At the moment I work on distribution and try to combine my work and study. In the Future, I would like to connect my life with frontend development.
4. I have good knowledge in HTML and CSS, and also excelled in JS. I started learning Git recently and I am new to this issue.
5. Completed a lot of tasks from Codewars  
example of one of the tasks:
*DESCRIPTION*:
-----------------
One of the common ways of representing color is the RGB color model, in which the Red, Green, and Blue primary colors of light are added together in various ways to reproduce a broad array of colors.

One of the ways to determine brightness of a color is to find the value V of the alternative HSV (Hue, Saturation, Value) color model. Value is defined as the largest component of a color:

V = max(R,G,B)
You are given a list of colors in 6-digit hexidecimal notation #RRGGBB. Return the brightest of these colors!

For example,

brightest(["#001000", "#000000"]) == "#001000"
brightest(["#ABCDEF", "#123456"]) == "#ABCDEF"
If there are multiple brightest colors, return the first one:

brightest(["#00FF00", "#FFFF00", "#01130F"]) == "#00FF00"
Note that both input and output should use upper case for characters A, B, C, D, E, F.

*task solution*
-------------------

function brightest(colors) {
  let result = colors.map(item =>
  item.slice(1)).map(item => item.split(''))
  let res = 0
  let n = 0;
  function spl(arr) {
    let a = [0]
    let b 
    let g = 0
    let j = 1
    for(let i = 0; i < 3; i++) {
      a[i] = arr[i + g] + arr[i + j];
      g++
        j++
      } 
    
    b = a.map(item => parseInt(item, 16))
    .sort((a, b) => b - a)[0]
    return b
  } 
  let index = 0
  let f = []
  for(let i = 0; i < result.length; i++) {
   f[i] = spl(result[i])
   if(f[i] > f[index]) {
     index = i
   }
   
  }
  
  return colors[index]
}

alert(brightest(['#00FF00', '#FFFF00' ]) )

6. No experience in commercial projects. He was only involved in the development of training tasks.

7. 1) Courses from SkillBox
   2) Higher technical education

8. English level B-1
