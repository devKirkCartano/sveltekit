<script>
    import {page} from '$app/stores';

    const greetings = {
        en: 'Hello',
        es: 'Hola',
        fr: 'Bonjour',
        de: 'Hallo',
        it: 'Ciao',
        pt: 'Olá',
    }
    const {lang = 'en'} = $page.params;
</script>

<h1>{greetings[lang]}</h1>