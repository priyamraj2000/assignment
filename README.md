# assignment(Below is code for given assignment in JavaScript)



function solution(D){
    let ans={'Mon':0,'Tue':0,'Wed':0,'Thu':0,'Fri':0,'Sat':0,'Sun':0,};
    let hash = ['Sun','Mon','Tue','Wed','Thu','Fri','Sat'];
    let date;
    for(let i in D){
        date=new Date(i);
        ans[hash[date.getDay()]]+=D[i];
    }
    return ans;
}
let D = {'2020-01-01':4,'2020-01-02':4,'2020-01-03':6,'2020-01-04':8,'2020-01-05':2,'2020-01-06':-6,'2020-01-07':2,'2020-01-08':-2};
let Day=solution(D);
console.log(Day);
