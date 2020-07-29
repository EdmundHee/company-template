<template>
  <div class="relative">
    <div class="h-screen">
      <div class="flex flex-col">
        <!-- 
          Header Content ( Landing Page )

          PARAMETERS
          :imgURL (URL for Background)
          :header_txt ( Header Text )
          :second_header ( Header 2 Text)
          :descriptions ( Descriptions )
        -->
        <HeaderContent
          imgURL="https://assets.bonappetit.com/photos/5c366551f212512d0e6cefd0/16:9/w_2560%2Cc_limit/Basically-Coffee-0219-03.jpg"
          header_txt="The LEAD"
          second_header="Institute of Growth"
          descriptions="FullStack Web Development Workshop"
        ></HeaderContent>
        <!-- 
          About Content 

          PARAMETERS
          :imgURL ( URL for about us )
        -->
        <AboutContent imgURL="https://www.cornellsci.com/images/about-002.png">
          <template
            v-slot:about
          >LEAD, is the institute that focus on growth. We help those that want to change their career or upskill.</template>
        </AboutContent>

        <ServiceContent>
          <template v-slot:services>
            <!-- 

              Service 

              PARAMETERS

              :imgURL (image url)
            -->
            <Service imgURL="/img/icon1.png" title="Turn idea into Reality">
              <template v-slot:content>Help and guide to turn ideas into Applications</template>
            </Service>

            <Service imgURL="/img/icon2.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>

            <Service imgURL="/img/icon3.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>

            <Service imgURL="/img/icon4.png" title="Service Title">
              <template
                v-slot:content
              >Lorem ipsum, dolor sit amet consectetur adipisicing elit. Repellendus excepturi quisquam temporibus non nisi doloribus cumque cum molestiae odio velit ratione perspiciatis assumenda numquam quam porro, sed quasi quia possimus?</template>
            </Service>
          </template>
        </ServiceContent>

        <!-- 
          Portfolio
        -->
        <PortfolioContent>
          <template v-slot:portfolio>
            <!-- 
              Project

              PARAMETERS
              :imgURL ( img URL for Project )
              :name ( Name of the Project )
              :project ( Name of Project Type)
              :projectURL ( Link Address to project)
            -->
            <Project
              imgURL="https://github.githubassets.com/images/modules/logos_page/Octocat.png"
              name="Company Template"
              project="NuxtJS App"
              projectURL="https://github.com/EdmundHee/company-template"
            />
            <Project
              imgURL="https://github.githubassets.com/images/modules/logos_page/Octocat.png"
              name="Company Template"
              project="NuxtJS App"
              projectURL="https://github.com/EdmundHee/company-template"
            />
            <Project
              imgURL="https://github.githubassets.com/images/modules/logos_page/Octocat.png"
              name="Company Template"
              project="NuxtJS App"
              projectURL="https://github.com/EdmundHee/company-template"
            />
            <Project
              imgURL="https://github.githubassets.com/images/modules/logos_page/Octocat.png"
              name="Company Template"
              project="NuxtJS App"
              projectURL="https://github.com/EdmundHee/company-template"
            />
          </template>
        </PortfolioContent>
        <ContactContent
          address="Level 11, Menara KEN TTDI, No.37 Jalan Burhanuddin Helmi, Taman Tun Dr. Ismail"
          email="support@thelead.io"
          phone="6016-473 7281"
          imgURL="/img/lead-white-logo.png"
        />
      </div>
    </div>
  </div>
</template>
<script>
export default {
  head() {
    return {
      title: "The LEAD"
    };
  }
};
</script>