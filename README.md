# Tour Of Heroes

Projeto desenvolvido no estudo de Angular, no tutorial do site. (https://angular.io/tutorial/toh-pt0)<br>
Foi desenvolvido em sete etapas, nas quais eu vi:

## Etapa 0

- Criei a estrutura inicial do aplicativo usando a CLI Angular
- Aprendi que os componentes Angular exibem dados
- Usoi as chaves duplas de interpolação para exibir o título do aplicativo

## Etapa 1

- Usoi a CLI para criar um segundo HeroesComponent
- Exibi o HeroesComponent adicionando-o ao AppComponent shell
- Apliquei o UppercasePipe para formatar o nome
- Usei vinculação de dados bi-direcional com a diretiva ngModel
- Aprendi sobre o AppModule
- Importei o FormsModule no AppModule para que o Angular reconheça e aplique a diretiva ngModel
- Aprendi a importância de declarar componentes no AppModulee que a CLI o declarou

## Etapa 2

- O aplicativo Tour of Heroes exibe uma lista de heróis com uma visualização detalhada
- O usuário pode selecionar um herói e ver os detalhes desse herói
- Exibir uma lista *ngFor
- Incluir ou excluir condicionalmente um bloco de HTML *ngIf
- Alternar uma classe de estilo CSS com uma classe de ligação.

## Etapa 3

- Criei o arquivo HeroDetailComponent.
- Usei uma associação de propriedade para dar a classe pai HeroesComponentcontrole sobre a classe filho    HeroDetailComponent.
- Usei o @Input para disponibilizar a propriedade hero para vinculação pelo arquivo HeroesComponent.

## Etapa 4

- Refatorei o acesso a dados para a classe HeroService
- Registrei o HeroService como provedor de serviços no nível raiz para que ele possa ser injetado em qualquer lugar do aplicativo
- Usei o Angular Dependency Injection para injetá-lo em um componente
- Dei ao HeroService get data método uma assinatura assíncrona
- Descobri a biblioteca Observable do RxJSObservable
- Usei RxJS of() para retornar um observável de heróis simulados (Observable<Hero[]>)
- O ngOnInit hook do ciclo de vida do componente para chamar o HeroService método, não o construtor
- Criei um MessageService para comunicação fracamente acoplada entre classes
- O HeroService injetado em um componente é criado com outro serviço injetado, MessageService

## Etapa 5

- Adicionei o roteador Angular para navegar entre diferentes componentes
- Transformei o AppComponent em um shell de navegação com <a> links e um <router-outlet>
- Configurei o roteador em um App-Routing-Module
- Defini rotas, uma rota de redirecionamento e uma rota parametrizada
- Usei a diretiva router Link em elementos âncora
- Você refatorou uma visualização mestre/detalhe fortemente acoplada em uma visualização de detalhes roteada
- Usei parâmetros de link do roteador para navegar até a visualização de detalhes de um herói selecionado pelo usuário
- Compartilhei o HeroServiceentre vários componentes

## Etapa 6

- Adicionei as dependências necessárias para usar HTTP no aplicativo
- Refatorei HeroService para carregar heróis de uma API da web
- Estendi HeroService para suporte aos métodos post(), put(), e delete() 
- Atualizei os componentes para permitir adicionar, editar e excluir heróis
- Configurei uma API da Web na memória
- Aprendi a usar observáveis