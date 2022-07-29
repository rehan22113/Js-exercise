# Js-exercise
i am sharing my own logic of javascript advanced concept
//infinite curring

function Add(a){
    return (function(b){
        if(b){return Add(a+b)}
        else{
            return a
        }
    })
}

console.log(Add(2)(2)(4)(3)())
