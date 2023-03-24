<template>
    <div class="container">
        <div class="item miles">
            <h3>Miles</h3>
        </div>
        <div class="item gwen">
            <h3>Gwen</h3>
        </div>
        <div class="item iron">
            <h3>Peter</h3>
        </div>
        <div class="item symbiote">
            <h3>Symbiote</h3>
        </div>
    </div>
</template>

<script>

</script>


<style scoped>
    .container{
        width: 900px;
        height: 500px;
        margin: 50px auto;
        display: flex;
        position: relative;
    }
    .item{
        width: calc(100% / 4);
        border: 1px solid black;
        height: 100%;
        background-repeat: no-repeat;
        filter: opacity(0.8);
        transition: all 0.8s;
        position: relative;
    }
    .miles {
        background-image: url(/public/miles_morales.jpg);
        background-size: 285%;
        background-position: -219px 0px;
    }
    .gwen {
        background-image: url("../../public/spider gwen.jpg");
        background-size: 232%;
        background-position: -142px 0px;
    }
    .iron {
        background-image: url("../../public/Spiderman_iron_suite.jpg");
        background-size: 169%;
        background-position: -80px 0px;
    }
    .symbiote {
        background-image: url("../../public/spidermn symbiote.jpg");
        background-size: 285%;
        background-position: -177px 0px;
    }
    h3 {
        position: absolute;
        bottom: 20px;
        left: 20%;
        color: white;
        text-shadow: black 1px 1px;
        font-size: 40px;
        display: none;
    }
    .item:hover {
        filter: opacity(1);
        scale: 0.9;
    }
    .item:active {
        width: 50%;
        z-index: 1;
    }
    .item:active h3 {
        display: block;
    }

</style>