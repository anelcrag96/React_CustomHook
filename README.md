# Notas Hooks

Este repositorio contine varios Custom Hooks para ayudarme a mi y a quien le sirvan.
La idea es que no tengamos que volver a escribirlos.

## ¿Qué son los Hooks en React?

Son funciones que permiten enganchar nuestros componentes funcionales a características propias de un componente de clase. Es decir, proporcionan un estado y un ciclo de vida a estos componentes evitándonos a los desarrolladores el uso de las clases.

## ¿Qué es un Custom Hook personalizado?

Son un mecanismo para reutilizar lógica de estado (como configurar una suscripción y recordar el valor actual), pero cada vez que usas un Hook personalizado, todo estado y efecto dentro de este son aislados completamente.

### useCounter

Ejemplo de uso:
```
    const { counter, increment, decrement, reset } = useCounter( 10 );
```

useCounter() //Recibe un valor por defecto

### useFetch

Ejemplo de uso:
```
    const url = 'EndPoint de API';
    const { data: null, loading: true, error: null } = useFetch( url );
```

### useForm

Ejemplo de uso:
```
    const initialForm = {
        name: '',
        age: 0,
        email: ''
    };

    const { formValues, handleInputChange, reset } = useForm( initialForm );
```

## Documentación React

Consulta más información en [https://es.reactjs.org/](https://es.reactjs.org/)