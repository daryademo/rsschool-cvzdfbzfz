Darya Tonk
tonk.darya@gmai.com
QA Engineer
HTML, CSS, JavaScript + Cypress, Python + Selenium, Java, SQL, JQuery, Jira, Trello, Figma, Balsamiq, TestRail
Northcentral Technical College 


https://www.codewars.com/kata/58291fea7ff3f640980000f9:
function allContinents(list) {
  let arrContinents = list.map(el=>el.continent)
  return arrContinents.includes('Africa' && 'Americas' && 'Asia' && 'Europe' && 'Oceania') 
  }



https://www.codewars.com/kata/57bf599f102a39bb1e000ae5
var fibsFizzBuzz = function(n) {
  if (n===1){
    return [1]
  }
  let arr=[1,1]
  for(let i = 2; i<n; i++){
    arr.push(arr[i-1]+arr[i-2])
  }
  return arr.map(el => el%15 ===0? 'FizzBuzz':
                 el%3 ===0? 'Fizz':
                 el%5 ===0? 'Buzz':
                el)
}


https://www.codewars.com/kata/589ace5eeef39faf49000061:
function reverseParentheses(s) {
  let res = ''
  let par = []
  for (let i = 0; i<s.length; i++){
    
    if (s[i] !== '(' && s[i] !== ')' ){
      res += s[i]
      
    } else if (s[i] === '('){
      par.push(res)
      res = ''
    } else if (s[i] === '('){
      par.push(res)
      res = ''
    } else if (s[i] === ')'){
      res = par.pop() + res.split('').reverse().join('')
    }
  }
  return res
}
