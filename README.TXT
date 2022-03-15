https://www.youtube.com/watch?v=GSlGO7KyX88



https://mapadevweek.com/aula-exclusiva/
DEV2022

const pokemonsCard = document.querySelectorAll('.cartao-pokemon')

listaSelecaoPokemons.forEach(pokemon => {
    //4- Precisamos trabalhar com um evento de clique feito pelo usuário na listagem de pokemons.
    pokemon.addEventListener('click', () => {
        console.log(pokemon)
        //remover a classe aberto só do cartão que está aberto.
        const CartaoPokemonAberto = document.querySelector('.aberto')
        CartaoPokemonAberto.classList.remove('aberto')

        //ao clicar em um pokemon da listagem, pegamos o id desse pokemon para saber qual cartão mostrar.
        const idPokemonSelecionado = pokemon.attributes.id.value

        const CartaoPokemonParaAbrir = 'cartao-' + idPokemonSelecionado
        const CartaoPokemonParaAbrir = document.getElementById('cartao-' + idPokemonSelecionado)
        CartaoPokemonParaAbrir.classList.add('aberto')

        //remover a classe ativa que marca o pokemon selecionado.
        const pokemonAtivoNaListagem = document.querySelector('.ativo')

        //adicionar a classe ativo no item selecionado.
        const pokemonSelecionadoNaListagem = ddocument.getElementById(idPokemonSelecionado)
        pokemonAtivoNaListagem.classList.add('ativo')