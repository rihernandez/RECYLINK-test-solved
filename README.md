# Prueba Algoritmica completada - RECYLINK (Desarrollador Full-Stack)

### Informacion personal
- Richard Hernandez
- rhc921004@gmail.com
- +1 (829) 904 7782


### Solucion :



## 1. Composite function

```javascript
function rokket(arg1) {
    return function(arg2) {
        return  function (arg3){
            return  console.log(arg1 + arg2 +arg3);
        }
    };
}

add(1)(2)(8);
```

## 2. Longest string

```javascript
function rokket(array) {
    let longestWord = "";
  
    array.forEach(function(word) {
      if(word.length > longestWord.length) {
        longestWord = word;
      }
    });
  
    return longestWord;
}
  
  var longest = rokket(['best', 'company', 'ever']);
  console.log(longest); 
```

## 3. String repetition

```javascript
  const rokket = (word, time) => {
    let repeatedWord = word.repeat(time); 
    let res = repeatedWord;
    console.log(res);
  }

  rokket("Hello",5);
```


## 4. Only last names

```javascript
  const rokket = (contacts) => {

    const contactsByLastName = [];
    contacts.forEach(function(contact) {
        contactsByLastName.push(contact.lastName)
    });
    console.log(contactsByLastName);

  }


    const contacts = [
        { firstName: 'Juanito', lastName: 'Rokket' },
        { firstName: 'James', lastName: 'Bond' },
        { firstName: 'Harry', lastName: 'Potter' } ]

  rokket(contacts);
```

## 5. Unique numbers

```javascript
const rokket = (array1,array2) => {
    const array3 = array1.concat(array2);
    
    const delDuplicates = (arr) => {
        return arr.filter((value, index) => {
          return arr.indexOf(value) === index;
        });
    }
    console.log(delDuplicates(array3));
}


rokket([1, 2, 5], [2, 1, 6]) 
rokket([1, 2, 3], [4, 5, 6])
```