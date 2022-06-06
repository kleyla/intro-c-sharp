### Métodos de strings

**Clone()**

```cs
string SchoolClone = School.Clone().ToString();
Console.WriteLine(SchoolClone);
```

El método Clone() crea un clon exacto de un string en una variable de tipo objeto. Por ello es necesario convertirlo a string utilizando ToString().

**CompareTo()**

```cs
Console.WriteLine(ClassTopic.CompareTo(School));
Console.WriteLine(School.CompareTo(SchoolClone));
```

Sirve para comparar el contenido de dos strings. Si son iguales devuelve 0 para true y si son diferentes retorna 1 para false. En este caso como School y SchoolClone son strings idénticos devolverá un 0. ¿Qué crees que se imprima en la primera línea?

**Contains()**

```cs
Console.WriteLine(School.Contains("Pla"));
```

Retorna True si el string contiene los caracteres que se pongan en los argumentos del método.

**EndsWith()**

```cs
Console.WriteLine(School.EndsWith("zi"));
```

Similar a Contains(), pero para comparar si los caracteres están al final del string.

**StartsWith()**

```cs
Console.WriteLine(School.StartsWith("Pl"));
```

Funciona de la misma manera que EndsWith(), pero en este caso comprueba si empieza con una serie de caracteres indicados.

**Equals()**

```cs
Console.WriteLine(School.Equals(SchoolClone));
```

Funciona de forma parecida a CompareTo(), pero para indicar si el contenido de ambos strings retorna True o False.

**IndexOf()**

```cs
Console.WriteLine(School.IndexOf("a"));
```

Regresa la posición dentro del string del carácter indicado en el argumento.
**ToLower() y ToUpper()**

```cs
Console.WriteLine(ClassTopic.ToLower());
Console.WriteLine(ClassTopic.ToUpper());
```

Convierten el string en todas letras minúsculas o mayúsculas.

**Insert()**

```cs
Console.WriteLine(School.Insert(6, " es educación online efectiva"));
```

Inserta un nuevo string dentro de otro en la posición indicada dentro de los argumentos. En este caso es en 6 que es la posición después de la última letra de “Platzi”.

**LastIndexOf()**

```cs
Console.WriteLine(ClassTopic.LastIndexOf("s"));
```

Regresa la posición de la última vez que aparece el carácter. En este caso la letra “s” aparece varias veces en el string y así podemos notar cómo devuelve la última posición en la que aparece.

**Remove()**

```cs
Console.WriteLine(ClassTopic.Remove(6));
```

Elimina los caracteres del string a partir de la posición que le indiquemos hasta el final.

**Replace()**

```cs
Console.WriteLine(ClassTopic.Replace("s", "z"));
```

Reemplaza todos los caracteres por otro indicado. En este caso todas las “s” serán cambiadas por “z”.

**Split()**

```cs
string[] split = ClassTopic.Split(new char[] { 's' });
Console.WriteLine(split[0]);
Console.WriteLine(split[1]);
Console.WriteLine(split[2]);
```

Este es un caso especial donde creamos un nuevo string donde guardamos el string separado en trozos por la letra indicada en los argumentos del método. Para este caso se separa por la letra “s” en 3 trozos que son los que imprimimos.

**Substring()**

```cs
Console.WriteLine(ClassTopic.Substring(2,10));
```

Devuelve un substring o trozo de string de acuerdo a las posiciones indicadas en los argumentos.

**ToCharArray()**

```cs
School.ToCharArray();
```

Convierte el string en un arreglo de caracteres.

**Trim()**

```cs
string TextWithSpaces = " hola, había espacios al principio y al final ";
Console.WriteLine(TextWithSpaces.Trim());
```

Elimina espacios al principio y al final de un string.
