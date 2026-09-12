<template>
    <div>
        <header>
            <p>Seja bem vindo:{{ nome }}</p>
            <img 
             width="200"
             :height="altura"
             :src="urlImgFluminense">
        </header>
    </div>
</template>

<script>
export default{
    name: "HomeComponent",
    data() {
        return{
            nome:"Mellyssa",
            altura:200,
            urlImgFluminense:
            "https://images.seeklogo.com/logo-png/5/2/fluminense-football-club-logo-png_seeklogo-56024.png"
        };
    },
    mounted(){
        setTimeout(()=>{
            this.urlImgFluminense= "https://static.vecteezy.com/system/resources/previews/009/267/561/non_2x/user-icon-design-free-png.png"
        }, 5*1000);
    }
};
</script>
