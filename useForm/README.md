# useForm Hook

Ejemplo de uso:

```
const initialForm = {
    name: '',
    age: 0,
    email: ''
}

const [formValues, handleInputChange, reset] =  useForm(initialForm)

```
NOTAS:

1- initialForm() retorna un array [objeto, funcionInput, funcionReset]
2- recuerde que los input del formulario deben cobtener los "name" respectivos

ejemplo: 
```
<label
                  htmlFor="email"
                  className="block text-sm font-medium leading-5 text-left text-gray-700"
                >
                  Email
                </label>
                <div className="mt-1 rounded-md shadow-sm">
                  <input
                    name="email"
                    type="email"
                    autoComplete="off"
                    value={email}
                    onChange={handleInputChange}
                    required
                    className="block w-full px-3 py-2 placeholder-gray-400 transition duration-150 ease-in-out border border-gray-300 rounded-md appearance-none focus:outline-none focus:shadow-outline-blue focus:border-blue-300 sm:text-sm sm:leading-5"
                  />
                </div>
                ```
