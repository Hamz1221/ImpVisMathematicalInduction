<template>
    <div>
        <iv-visualisation :title="pageName" :vue_config="vue_config" :page_number="2">
                        <iv-pane position="left" format="overlay" :width=30>
                <iv-sidebar-content>
                    <iv-sidebar-section title="The Game of Frogs">
                        <h1>Have at it!</h1>
                        <p>
                            There are infinite possible starting configurations for the game - take the time to experriment
                            yourself. Use the sliders to control the frogs' speeds and click on them to change their directions.
                        </p>
                        <p>
                            Are the frogs always doomed to fall or is there a case where they can bounce around forever?
                        </p>
                        
                    </iv-sidebar-section>
                </iv-sidebar-content>
            </iv-pane>
        </iv-visualisation>
    </div>
</template>
<script>
import vue_config from '../../vue.config.js'
export default {
    name:"page_2",
    data(){
        return {
            pageName:"Page 2",
            vue_config
        }
    }
}
</script>
<style>
.iv-welcome-message{
    display:flex;
    flex-direction: column;
    align-items: center;
    margin-top: 50px;
}
</style>