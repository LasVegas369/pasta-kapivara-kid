// Para personagem tiringa agachar (lembrando que tem que ter a sprite para agachar)
const tiringa = document.getElementById('tiringa');

function tiringaAgachar() {
    tiringa.classList.add('agachando');
}

function tiringaLevantar() {
    tiringa.classList.remove('agachando');
}

document.addEventListener('keydown', (event) => {
    if (event.key === 'Control' || event.key === 'ArrowDown') {
        tiringaAgachar();
    }
});

document.addEventListener('keyup', (event) => {
    if (event.key === 'Control' || event.key === 'ArrowDown') {
        tiringaLevantar();
    }
});
