<template>
    <!-- Wrapper -->
    <div class="wrapper">
        <StartedSectionComponents/>

        <ServicesComponents/>

        <SkillComponents/>            

        <PortfolioComponents/>

        <ResumeComponents />

        <BlogComponents />

        
        <ContactComponents />
        

           

    </div>
</template>
<script>
import StartedSectionComponents from '@/components/StartedSectionComponents.vue'
import ServicesComponents from '@/components/ServicesComponents.vue'
import SkillComponents from '@/components/SkillComponents.vue'
import PortfolioComponents from '@/components/PortfolioComponents.vue'
import ResumeComponents from '@/components/ResumeComponents.vue'
import BlogComponents from '@/components/BlogComponents.vue'
import ContactComponents from '@/components/ContactComponents.vue'
export default {
    name: 'HomeView',
    components: {
        StartedSectionComponents,
        ServicesComponents,
        SkillComponents,
        PortfolioComponents,
        ResumeComponents,
        BlogComponents,
        ContactComponents
    }
    
}
</script>