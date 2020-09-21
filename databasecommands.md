[1]How to get database ->

- firebase.database();

1)create a var to store it

- var database = firebase.database();

[2]How to get reference for database or a particular node->

1)first get ref of database

- database.ref('/');

2)this will refer to the entire data base

- database.ref('<nodename>');

3)<nodename> is the name of the node we want to refer

[3]How to get a value from database ->

- database.ref('<nodename>').on("value",function(data){
  <variablename> = data.val();
});

[4]How to set the data ->

- database.ref('<nodename> or /').set({
    <nodename> : <value(whatever value we want to update)>
});

[5]How to update the data ->

- database.ref('<nodename> or /').update({
    <nodename> : <value(whatever value we want to update)>
});