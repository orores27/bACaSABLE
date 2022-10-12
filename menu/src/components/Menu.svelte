<script>
	

    
</script>


    <nav>
        <div class="img">
            <img src="img/img.svg"/>
        </div>
        <ol>
            <slot />
        </ol>
    </nav>


<style lang="scss">
    nav {
        display: flex;
		flex-direction: column;
		align-items: flex-start;
		width: 150px;
        height: 100%;
        background-color: rgb(222, 204, 239);
        
        }
        .img {
            display: flex;
            justify-content: center;
            width: 50%;
            margin-top: 20px;
            margin-left: 30px;   
        }
        img {
            width: 100%;
 
        }
            ol {
                width: 20%;
                margin-top: 40px;
                padding-left: 0;
            }
</style>