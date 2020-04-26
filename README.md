# Projeto de estudo de React

----

### Etapas
1. Conhecendo o React
2. Configurar o ambiente de estudo
3. Adicionando os 'scripts CDN react e reactDom' no documento principal

> ```html
> <script crossorigin src="https://unpkg.com/react@16/umd/react.development.js"></script>
> <script crossorigin src="https://unpkg.com/react-dom@16/umd/react-dom.development.js"></script>
> 
> ```
>
> 

4. Adicionando o interpretador 'Babel js'

> ```html
> <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
> ```
>
> 

5. Trabalhando com Function Component

> ```jsx
> function MeuComponent(){
>   return(
>     <div>
>     	<h1>Olá React Js</h1>
>     </div>
>   );
> }
> ```
>
> 

6. Trabalhando com Class Component

> ```jsx
> class MeuComponent extends React.Component{
>   render(){
>     <div>
>       <h1>Class Component</h1>
>     </div>
>   }
> }
> ```

7. Trabalhando com propriedades chamadas de "props" passando parâmetros dentro da função.

> ```jsx
> // Trabalhando com props dentro de uma function
> function CompProps(props){
>    return(
>      <div>
>        <p>Nome: {props.nome}</p>
>        <p>Apelido: {props.apelido}</p>
>      </div>
>    );
> }
> // Trabalhando com a props dentro de uma Class Component
> class CompProps extends React.Component{
>   render(){
>     <div>
>       <p>Nome: {Nome: {this.props.nome}}</p>
>       <p>Apelido: {Apelido: {this.props.apelido}}</p>
>     </div>
>   }
> }
> 
> ReactDOM.render(
>   <CompProps nome='Wendel Lopes' apelido='Develop Man' />,
>   root
> );
> ```

8. Usando style CSS dentro do React.

> Como o intuito de usar os recursos do 'css' dentro do React não podemos usar a palavra class, pois é uma palavra reservada do React, fazendo-se então necessário a utilização da palavra chave "className".
>
> ```jsx
> class StyleComponent extends React.Component{
>    render(){
>       return(
>          <div className='container has-background-primary'>
>             <h1 className='title has-text-white'>Develop Ruby on Rails</h1>
>             <h3 className='subtitle has-text-white'>e React Js</h3>
>          </div>
>       );
>    }
> }
> ```
>
> 

9. Introdução ao conceito de { state } dentro do React, onde podemos definir valores internos dentro de nosso componentes.

> Para a utilização do { state } é necessário que sua declaração seja feita dentro de um { construtor }.
>
> ```jsx
> class App extends React.Component{
> 
>   constructor(){
>     super();
> 
>     this.state = {
>       sistema: 'Linux Pop!',
>       versao: '20.2.9p'
>     }
>   }
> 
>   render(){
>     return(
>       <div className='container' style={{padding:'20px'}}>
>         <p>Sistema: {this.state.sistema}</p>
>         <p>Versão: <small> {this.state.versao} </small></p>
>       </div>
>     );
>   }
> }
> ```
>
> 

