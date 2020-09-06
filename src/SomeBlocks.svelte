<script>
    function toggle() {
        let opacity = this.style.opacity;
        if (opacity === "0") {
            document.querySelectorAll(".block").forEach(element => element.style.opacity = "1");
        } else {
            this.style.opacity = "0";
        }
    }
</script>
<style>
    .block {
        width: 100px;
        height: 100px;
    }
    .red {
        background-color: red;
    }
    .blue {
        background-color: blue;
    }
    .green  {
        background-color: green;
    }
</style>
<div>
    <div on:click={toggle} class="block red"></div>
    <div on:click={toggle} class="block blue"></div>
    <div on:click={toggle} class="block green"></div>
</div>