<template>
    <div class="container">
        <div class="row">
            <div class="col-md-8 col-md-offset-2">
                <div class="panel panel-default">
                    <div class="panel-heading">Client Units</div>

                    <div class="panel-body">
                        <table class="table">
                            <thead>
                                <tr>
                                    <th>UUID</th>
                                    <th>Name</th>
                                    <th>Range</th>
                                </tr>
                            </thead>
                            <tbody>
                                <tr>
                                    <td>1lk2jsdkjl324-aslkjklw2-sdfoiu9riw</td>
                                    <td>Rikards Beacon</td>
                                    <td>22534, 2313</td>
                                </tr>
                            </tbody>
                        </table>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        ready() {
            console.log('Component ready.')

            this.$http.get('/api/user')
                .then(response => {
                    console.log(response.data);
                });
        }
    }
</script>
