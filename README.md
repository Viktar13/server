# server

server for study

new line
const express = require('express');
const app = express();
// let name = "Viktar";
// let i = 0;
let names = ["Mama","Tata","Agata","Kot","Sabaka","Zabka"];


app.get('/', (req, res) => {
    let text = "<ol>";
    for(let i =0;i<names.length;i++){
        text=text+"<li>"+names[i]+"</li>";
    }
    text=text+"</ol>";
    console.log(text)
    res.send(text);
})
app.listen(3000);
