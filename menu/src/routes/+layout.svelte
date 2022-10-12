<script>
    import Menu from "../components/Menu.svelte";
    import MenuItem from "../components/MenuItem.svelte";
    import { page } from '$app/stores';
</script>


    <div class="container">
        <div class="menu-container">
            <div class="menu">
                <Menu>
                    <MenuItem nom="Home" href="/" img="img/home.svg" selected={$page.url.pathname === "/"}/>
                    <MenuItem nom="Growing" href="/growing" img="img/icon1.svg" selected={$page.url.pathname === "/"}/>
                    <MenuItem nom="Pinned File" href="/pinned_file" img="img/icon2.svg" selected={$page.url.pathname === "/pinned_file"}/>
                    <MenuItem nom="Search File" href="/search_file" img="img/icon3.svg" target="_blank"/>
                    <MenuItem nom="Delete" href="/delete" img="img/icon4.svg" target="_blank"/>
                    <MenuItem nom="Archive" href="/archive" img="img/icon5.svg" target="_blank"/>
                </Menu>
            </div>
        </div>
    </div>
    <slot />

    <style>
        .container {
            display: flex;
        }
        .menu-container {
            width: 160px;
        }
        .menu {
            position: fixed;
            display: flex;
            flex-direction: column;
            height: 100vh; 
        }
    </style>

    