# Regular Expressions (RegEx)
### Para que utilizar
Você pode usar o regex para verificar se um texto segue certo padrão, retornando `true` ou `false` para confirmar se um texto (`string`) está conforme deve estar

# Retorno de boolean
#### Javascript
```javascript
  const regexString = "/^([0-9... $/"
  const string = "abc123"
  var bool = regexString.test(string)
```
#### Java
```java
  String regexString = "/^([0-9... $/";
  String string = "abc123";
  boolean allGood = string.matches(regexString);
```
# Regex úteis

### Dinheiro
```javascript
/^(R\$\s?\d)(\,\d{2}|\.\d{2})?$/
```

### Telefone
```javascript
/^((\(\d{2}\)|\d{2})(\9\d{4}\-?\d{4}|[1-8]\d{3}\-?\d{4}))$/
```

### CEP
```javascript
/^(\d{5}\-?\d{3})$/
```

### CPF
```javascript
/^(\d{3}\.\d{3}\.\d{3}\-\d{2}|\d{3}\d{3}\d{3}\d{2})$/
```

### CNPJ
```javascript
/^(\d{2}\d{3}\d{3}\d{4}\d{2}|\d{2}\.\d{3}\.\d{3}\/\d{4}\-\d{2})$/
```

### Horário 24h
```javascript
/^([0-1]?[0-9]|2[0-4]):([0-5][0-9])(:[0-5][0-9])?$/
```

### Email
```javascript
/^(([^<>()[\]\\.,;:\s@"]+(\.[^<>()[\]\\.,;:\s@"]+)*)|(".+"))@((\[[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\.[0-9]{1,3}\])|(([a-zA-Z\-0-9]+\.)+[a-zA-Z]{2,}))$/
```

### URL Link
```javascript
/^(https\:\/\/)?(www\.)?[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)$/
```
ou
```javascript
/[-a-zA-Z0-9@:%._\+~#=]{1,256}\.[a-zA-Z0-9()]{1,6}\b([-a-zA-Z0-9()@:%_\+.~#?&//=]*)/
```

### Data (dd/mm/yyyy)
```javascript
/(^(((0[1-9]|1[0-9]|2[0-8])[\/](0[1-9]|1[012]))|((29|30|31)[\/](0[13578]|1[02]))|((29|30)[\/](0[4,6,9]|11)))[\/](19|[2-9][0-9])\d\d$)|(^29[\/]02[\/](19|[2-9][0-9])(00|04|08|12|16|20|24|28|32|36|40|44|48|52|56|60|64|68|72|76|80|84|88|92|96)$)/
```
