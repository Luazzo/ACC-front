<template>
    <!--Image HEAD -->
    <div class="page-header page-header-small">
        <parallax class="page-header-image"
                  style="background-image: url('img/presentation-page/liege-atlas.jpg'); background-position: top 20px center;">
        </parallax>
        <div class="contentcenter">
            <div class="row">
                <div class="col-md-8 ml-auto mr-auto text-center">
                    <h1 class="title">L'Assurence, simplement...</h1>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        name: "HeadImage"
    }
</script>

<style scoped>
    .contentcenter {
        position: absolute;
        top: 78%;
        left: 50%;
        z-index: 2;
        -webkit-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
        text-align: center;
        color: #FFFFFF;
        padding: 0 15px;
        width: 100%;
        /*max-width: 880px;*/
    }

</style>
