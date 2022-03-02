<template>
    <div>
        <iv-visualisation :title="pageName" :vue_config="vue_config" :page_number="1">
            <iv-pane position="left" format="overlay" :width=30>
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
                    <iv-sidebar-section title="The Game of Frogs">
                        <h1>In The Game of Frogs, you swim or you die</h1>
                        <p>
                            Let there be n frogs lines up on a frictionless log. All the frogs start moving with a nonzero velocity.
                            When two frogs collide they bounce off each other, and when they reach the end of the log they fall off
                            into the water and are removed from the game.
                        </p>
                        <p>
                            In this case, n=5 and the frogs are positioned as seen on the right. What do you think will happen as 
                            time unfolds?
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
</style>