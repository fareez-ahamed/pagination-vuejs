<template>
<div class="container">
    <div id="app" class="well">
        <h1>This is page {{pageOne.currentPage}}</h1>
    </div>
    <pagination :current-page="pageOne.currentPage"
                :total-pages="pageOne.totalPages"
                @page-changed="pageOneChanged">
    </pagination>
</div>

</template>

<script>
import Pagination from './Pagination.vue'

export default {

    components : { Pagination },

    data() {
        return {
            pageOne: {
                currentPage: 1,
                totalPages: 10
            }
        }
    },

    methods: {
        pageOneChanged (pageNum) {
            this.pageOne.currentPage = pageNum
        }
    }
}
</script>

<style>
body {
    font-family: Helvetica, sans-serif;
    padding-top: 80px;
}
</style>
