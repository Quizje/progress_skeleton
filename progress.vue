<template>
    <div></div>
</template>

<script>
    const axios = require('axios')

    export default{
        props: {

        }
        methods: {
            makeRequest() {
               axios.get('/url?params=12345')
                .then(function (response) {
                    // handle success
                    console.log(response);
                })
                .catch(function (error) {
                    // handle error
                    console.log(error);
                })
                .then(function () {
                    // always executed
                });
            }
        }
    }
</script>
