<template>
        <div id="body" data-spy="scroll" data-target=".header">
            <topBox></topBox>
            <bannerBox></bannerBox>
            <mySkills></mySkills>
            <experience></experience>
            <work></work>
            <Contact></Contact>
            <bottomBox></bottomBox> 
        </div>
        </template>
        
        <script>
        import topBox from '../components/head';
        import bottomBox from '../components/footer';
        import bannerBox from '../components/banner';
        import mySkills from '../components/mySkills';
        import Contact from '../components/contact';
        import work from '../components/work';
        import experience from '../components/experience';
        export default {
        name: 'aboutMe',
        data () {
            return {
            msg: 'Welcome to Your Vue.js App'
            }
        },
        components:{
            topBox,
            bannerBox,
            mySkills,
            experience,
            work,
            Contact,
            bottomBox
        }
        }
        </script>
        
        <!-- Add "scoped" attribute to limit CSS to this component only -->
        <style scoped>
        
        </style>
              