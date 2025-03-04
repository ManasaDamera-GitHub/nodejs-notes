# nodejs-notes

to perform operations on files, we have to use fs module.
require("fs--->it will imports the fs module in our project.


performs asynchronous operations on file
fs.readFile(path of the filename,"utf8")
fs.writeFile(path of the filename,"data")
fs.appendFile()
fs.unlinksync()

performs synchronous way wehn u use
readFileSync()
fs.writeFileSync(filename,"data")
fs.appendFileSync()
fs.unlinksyncSync()





const fs=require("fs")
const express=require("express")

const app=express();

app.get("/get",(req,res)=>{
res.set("content-type","application/json");  // adding headers using set method
res.send("hello");


re.readFile("./hello.txt","utf8",(err,data)=>{
if(err){
res.send(err);
}
else{
res.send(data)
}
})

difference between read file and appendFile:

readFile will replace the old data with new data.if there is no file exist then it will create and add data in that file.where as append file will add new to to the old data.












}

