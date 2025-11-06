class Livro{
    constructor(public titulo:String,public disponivel: Boolean= true)}

}
 class biblioteca {
    private livros:Livro;

    adicionardLivro(livro:livro){
        this.livros.push(livro);
    } 
   async emprestar(titulo:String):Promise<void>{
    return new Promise((resolve,reject))=>{
        const livro=this.livros.find(l=.titulo===titulo);
        if(livro){
            return reject(new console.error("livro não encontrado" na biblioteca!));

            )
            if(!livro.disponivel){
                return reject(new error("livro já esta empretado"));

            }
        }
       livro.disponivel=false;
       console.log('você emprestou:"${livro.livro}"');
       resolve();
    });
    {
        async devolver(titulo:String):Promise>void{
            return new Promise((resolve , reject))=>{
                const livro=this.livros.find(l=.titulo===titulo);

                if (!livro){
                    return reject(newe error( "este livro não  pertence a biblioteca! "));

                }
            if(!livro.disponivel){
                return reject(new error("Este livro já foi devolvido!"));
                {
                    livro.disponivel=true;
                    console.log(´ você devolveu:"${livro.titulo}");
                    rosolve():
                
                }
            }
              
            }
         async function () {
            const biblioteca=new biblioteca();

            // Criando livros
            biblioteca.adicionardLivro(new livro("introdução nutrição");
            biblioteca.adicionardLivro(new livro("Harry potter ");
            biblioteca.adicionardLivro(ne("pequeno manual antirracista");

            try{
           await biblioteca.emprestar("introdução nutrição");
           await biblioteca.emprestar("introdução nutrição");// vai gerar
           
           error
           {.catch(erro:any)
            console.error(Erro:",erro.messagem );
           }
            }
            try
            await biblioteca.devolver("introdução nutrição");
            await biblioteca.devolver("harry potter");// vai gerar erro 
        }catch(erro: any){
            console.error("Erro",erro.message);
        }
         }
    } 
       main()
    }
   } 
 }# Projeto-da-biblioteca-
exercícios em sala de aula 
