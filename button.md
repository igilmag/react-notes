# Desestructuración de props

Podemos desestructurar las props y pasárselo como atributo a un componente. Incluso se pasan las propiedades __children__

```js
export const Button = ({ handleClick, ...props }) => {
  return (
    <button onClick={handleClick} {...props} />
  )
}
```
Utilización del componente

```html
<Button handleClick={handleLike} className='btn'>
  Like 
</Button>
```