Comandos React:

npm create vite@latest
nome do projeto
react
javascript
npm install
npm run dev

npm install json-server
npm run server

npm install axios

npm install react-router-dom
npm install @mui/material @emotion/react @emotion/styled

aplicações:
ES7+

obs:
Adicionar em package.json em "scripts" a seguinte propriedade:
 "server": "json-server --watch data/db.json"

GET:
 const [suppliers, setSuppliers] = useState([])

    useEffect(() => {
        axios.get('/suppliers')
        .then(response => {
            setSuppliers(responce.data)
        })
        .catch(error => console.error("Ocorreu um erro: ",error))
    }, []);