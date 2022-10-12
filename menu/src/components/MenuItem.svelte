<script>
    export let nom = "";
    export let href = "";
    export let img = '';
    export let selected = false;
    export let target = '';
</script>

    <div>
        <li>
            <a {href} {target}>
                <span class="img"><img src={img} alt="nom"/></span>{nom}
            </a>
        </li>
    </div>

<style>
    li {
        list-style: none;
        opacity: 70%;
        width: 100%;
    }
        a {
            display: flex;
            align-items: center;
			padding: 1em;
            width: 100%;
            
        }
        .img {
            display: flex;
            width: 100%;
        }
        img {
            width: 100%;
        }

    

</style>