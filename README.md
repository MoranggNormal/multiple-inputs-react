### This is a multiple inputs in React Form.

<pre>
import React, {useState} from 'react'

export default function Home() {

    const [stats, setStats] = useState({

    })

    const data =[
        {name: 'nome', type: 'text'},
        {name: 'cargo', type: 'number'},
        {name: 'birth', type: 'text'},
        {name: 'addres', type: 'text'},
        {name: 'bairro', type: 'text'},
        {name: 'cidade', type: 'text'},
        {name: 'cep', type: 'number'},
        {name: 'phone', type: 'number'},
        {name: 'contact', type: 'number'},
        {name: 'email', type: 'text'},
        {name: 'identity', type: 'text'},
        {name: 'cpf', type: 'number'},
        {name: 'isDriver', type: 'text'},
        {name: 'habilitacao', type: 'text'},
    ]

   /* const handleInputChange = (e) => {
        setStats({
            ...stats,
            [e.target.name]: e.target.value
        });
    }

   */


  return (
    <div>
        {data.map( ({name, type}, i) =>
               &lt;input
                    key={i}
                    name={name}
                    type={type}
                    placeholder={name}
                    onChange={(e) => setStats({[e.target.name]: e.target.value})} 
                /&gt;
        )}

        {stats.nome}
        {stats.cargo}
        {stats.addres}

    </div>
  )
}

</pre>
