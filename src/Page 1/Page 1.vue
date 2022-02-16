<template>
    <div>
        <iv-visualisation :title="pageName" :vue_config="vue_config" :page_number="1">
            <iv-pane position="left" format="overlay">
                <iv-sidebar-content>
                    <iv-sidebar-section title="Mathematical Induction">
                        <h1>Reasoning mathematically about programs</h1>
                        <p>
                            If we want to prove that a program produces the correct result,
                            a necessary step is to prove that it will finish running in a finite time at all!
                        <br>
                            It turns out this is far from trivial - there is no algorithm to find out if
                            any given program will terminate.
                        </p>
                        <p>
                            Despite this there are mathematical tools, like induction, that allow us to go a long
                            way in formally proving the behaviour of many specific programs.
                            Let's see a simple example of such a process: can you deduce whether it will terminate,
                            and more importantly justify your answer mathematically?
                        </p>

                        
                    </iv-sidebar-section>
                </iv-sidebar-content>
            </iv-pane>
            <div class="iv-welcome-message">
                <img src='@/assets/ImpVis-logo.png' alt="ImpVisLogo" height="50"/>
                <h1> Welcome to Imperial Visualisations!</h1>
                <p> Your page, Page 1 has succesfully been set up using the multiPage CLI template!</p>
            </div>
        </iv-visualisation>
    </div>
</template>
<script>
import vue_config from '../../vue.config.js'
export default {
    name:"page_1",
    data(){
        return {
            pageName:"Page 1",
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