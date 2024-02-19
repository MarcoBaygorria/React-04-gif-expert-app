# Gif Expert App
***

# Creando una lista de categorias
```
1. Para poder Barrer categorias utilizamos el map()
2. Después se crea una variable llamada category la cual con función de flecha se utiliza para retornar el li.
   Ej:           {categories.map(category => {
            return <li key={category}>{category}</li>
          })
          }

```
***

# Agregar un nuevo elemento a categories.
```
1. Primero creamos una función con el nombre de onAddCategory.
2. Creamos un button arriba del ol.
3. Utilizamos el onClick en el button y hacemos referencia a la función onAddCategory para enlazarlos.
4. Utilizamos setCategories para desestructurar categories y agregar el nuevo elemento.
   Ej: setCategories([...categories, 'Solo Leveling'])
```
***

# Componente AddCategory
```
1. Creamos una carpeta llamada components.
2. Dentro de la carpeta creamos un archivo llamado AddCategory.jsx
3. En el GifExpertApp.jsx en la parte del input vinculamos el AddCategory
   Ej: <AddCategory />
4. En el AddCategory.jsx en el return creamos el input, con sus respectivas características (type y placeholder).
5. creamos un useState de nombre inputValue. value={inputValue}
6. En value, dentro del input ponemos inputValue.
7. Creamos el método onChange={}que esta dentro del input.
8. Creamos una función de nombre onInputChange
9. La asociamos al onChange, asi quedaría = onChange={ onInputChange }
10. En el onInputChange, desestructuramos y obtenemos el target a lo cual en el setInputValue agregamos el targe.value
    Ej:     const onInputChange = ({target}) => {
                setInputValue(target.value);
            }
11. creamos un form el cual dentro tendrá el input. <form></form>
12. En el form creamos un onSubmit, quedaría asi: onSubmit={(event) => onSubmit(event)}
13. Creamos una función llamada onSubmit.
14. Para evitar el refresh del navegador web usamos lo siguiente.
    EJ:     const onSubmit = (event) => {
                event.preventDefault();
                console.log(inputValue);
            }
```
***

# Comunicación entre componentes
```

```