<template lang="pug">
//- section.top-area(style="padding: 16rem 1rem")
    .inner
        img(src="/assets/img/teklium.png" style="width: 17vw; min-width: 120px; margin-bottom: 2rem;")
        h1(data-aos="zoom-in" data-aos-duration="1000" style="font-size: 3rem") Teklium
        p(data-aos="fade-up" data-aos-duration="1200") Pioneering new environmentally sustainable technologies #[br] to revolutionize the way we live, work, and play.

//section.dark.blend(style="padding: 12rem 1rem;")
// compensate bottom padding
section.dark.blend.landingTop(style="padding: 9rem 1rem 4rem;min-height: 100vh;display: flex;align-items: center;")
    img.img-in-blend(src="/assets/img/chip.jpg")
    .inner
        .tit(style="display:flex; align-items:center;")
            // logo by height not width
            img(src="/assets/img/teklium.png" style="height: 2.5em; margin-right: 1rem;")
            h1(style="font-family: 'Arial';font-weight:300;font-size: 2.5rem;margin:0;") Teklium
        br
        // use h tags, strong for bold text within tags
        h2.yellow Innovating #[.wordset eco-friendly technologies] #[.wordset to transform everyday living,] #[.wordset working, and recreation.]
        //strong.yellow(style="font-size:1.1rem;") Innovating eco-friendly technologies to transform everyday living, working, and recreation.
        //p.ellipsis We are a seasoned team of scientists with extensive expertise in aerospace, mechanical engineering, energy, artificial intelligence, and semiconductor technology. Our team members have made significant contributions to advanced projects, including the F-35, the United States' most advanced jet fighter. With a proven track record of innovation and excellence in mechanical design, computer science, semiconductor technologies, and energy solutions, we are dedicated to pioneering advancements in these fields.
        p We are a seasoned team of scientists with extensive expertise in aerospace, mechanical engineering, energy, artificial intelligence, and semiconductor technology. Our team members have made significant contributions to advanced projects, including the F-35, the United States' most advanced jet fighter. With a proven track record of innovation and excellence in mechanical design, computer science, semiconductor technologies, and energy solutions, we are dedicated to pioneering advancements in these fields.
        br
        br
        //- button.fullButton(@click="router.push('/tech')") View more
        button.fullButton(@click="router.push('/tech')") View Technologies

//- section.serve(style="padding:5rem 1rem 6rem")
section.serve
    br
    //- .inner(style="text-align:center;")
    .inner
        // h1.blue Pioneering the Future #[br]of Semiconductor Technologies
        .sectionTitle(data-aos="fade-up") Pioneering the Future of #[.wordset Semiconductor Technologies]
        //- strong Revolutionizing Performance and #[span.wordset Efficiency with Carbon-Based Innovations]

        br

        .cardWrap.vision 
            .card(data-aos="fade-up")
                h3 Innovative Carbon Semiconductor Technology
                p
                    strong Solutions for Industrialization and the Digital World
                    | At Teklium, we address the increasing demands of industrialization, economics, science, education, and politics with our groundbreaking carbon semiconductor technology developed in partnership with Nantero and Visual Link. Unlike traditional silicon chips, our carbon semiconductors deliver superior performance, power efficiency, and heat dissipation, featuring multi-layered 3D semiconductor technology and Carbon Nanotubes (CNT), with a lifespan of up to 100 years.

            .card(data-aos="fade-up")
                h3 Creating Innovative Solutions for a Digital World
                
                p
                    strong Revolutionizing Data Center Operations and AI Applications
                    | With innovations such as the Reusable Chip, Memory-Mapped CPU, Quantum Communications, and Content Aware Memory, we are transforming data center operations and enhancing the speed, efficiency, and security of AI applications. Our vision for a Super Internet, featuring Quantum Spooling and Atomic Routing, aims to improve global internet infrastructure.

            .card(data-aos="fade-up")
                h3 Sustainable Business Strategies
                p
                    strong AI City and Chip Subscription Model
                    | AI City, supported by strategic partnerships, aims to enhance broadband accessibility, data center efficiency, and sustainable economic development. Additionally, our Chip Subscription model allows users to access the latest advanced chips on a subscription basis, reducing electronic waste and ensuring they remain up to date with cutting-edge technology.

    br
    br
    br
    
    //- .inner(style="margin-top: 11rem;")
    .inner
        //- h1(style="text-align:center") Who We Serve
        .sectionTitle(data-aos="fade-up") Who We Serve

        br

        .cont-wrap
            .wrap.ai(data-aos="fade-up")
                //- .image
                //-     img(src="/assets/img/ai.jpg" style="height: 200px")
                .content 
                    h2 Artificial Intelligence
                    p Our state-of-the-art AI processors and memory solutions meet the growing computational demands of data centers and AI-focused businesses.

            .wrap.ad(data-aos="fade-up" style='background-color: #263980;')
                //- .image
                //-     img(src="/assets/img/space.jpg" style="height: 200px")
                .content
                    h2 Aerospace and Defense
                    p We provide rugged, high-performance technologies tailored for military applications, drawing on extensive experience in aerospace and defense.

            .wrap.ce(data-aos="fade-up" style='background-color: #365d3e;')
                //.image 
                    img(src="/assets/img/electronic.jpg" style="height: 200px")
                .content
                    h2 Consumer Electronics
                    p We deliver next-generation computing power to consumer electronics, including smartphones and gaming consoles.

            .wrap.am(data-aos="fade-up" style='background-color: #9b2f26;')
                //- .image 
                //-     img(src="/assets/img/automotive.jpg" style="height: 200px")
                .content
                    h2 Automotive
                    p Our advanced in-car system processing power and autonomous driving capabilities are revolutionizing the automotive industry.

section.dark.blend(style='height: 70vw; max-height: 30vh;display:flex;align-items:center;justify-content:center;')
    .inner(data-aos="fade-up" style="text-align:center")
        h2(style='margin-top:0;') Leading the Way in Innovation#[br]Connecting Technology and the Future
        button.fullButton(@click="router.push('/tech')") View more
    br
</template>

<script setup>
import { useRoute, useRouter } from "vue-router";

const router = useRouter();
const route = useRoute();
</script>

<style scoped lang="less">
// .top-area {
//     padding-top: 15rem;
//     text-align: center;

//     h1 {
//         font-size: 4rem;
//         margin: 0;
//         background-color: #000106;
//         -webkit-background-clip: text;
//         -moz-background-clip: text;
//         background-clip: text;
//         color: transparent;
//         text-shadow: rgba(255, 255, 255, 0.5) 0px 3px 3px;
//         font-size: clamp(5rem, 23.8vw, 16rem);
//     }

//     p {
//         font-size: clamp(14px, 3.5vw, 1.5rem);
//     }
// }
.blend {
    position: relative;
    background-color: unset;

    &::after {
        position: absolute;
        content: "";
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        background-color: rgba(255, 255, 255, 0.85);
        mix-blend-mode: difference;
    }

    &.landingTop::after {
        background-color: rgb(93 96 103);
        mix-blend-mode: hue;
    }
    .inner {
        position: relative;
        z-index: 1;
    }
}
.serve {
    .wrap {
        // display: block;
        // flex: 1;
        // min-width: 270px;
        width: 480px;
        flex-grow: 1;
        flex-shrink: 1;

        // background-color: #f3f0e8;
        background-color: #352d33;
        // border-radius: 1rem;
        // border-radius: .5rem;
        // overflow: hidden;
        box-shadow: 0 2px 20px 0 rgba(0, 0, 0, .1);

        > div {
            min-width: initial;
            width: 100%;
        }

        display: flex;
        align-items: end;
        
        .content {
            // padding: 0 2rem 1rem;
            padding: 50% 2rem 1rem;
            
            h2, p {
                color: white;
            }

            background: linear-gradient(0deg, black, transparent);
        }
        
        background-size: cover;
        background-position: 15% 100%;

        &.ce {
            background-image: url("/assets/img/electronic.jpg");
        }
        &.ai {
            background-image: url("/assets/img/ai.jpg");
        }
        &.ad {
            background-image: url("/assets/img/space.jpg");
        }
        &.am {
            background-image: url("/assets/img/automotive.jpg");
        }
    }
}
.cont-wrap {
    display: flex;
    flex-wrap: wrap;
    // gap: 2rem;
    gap: 1rem;
    // margin-top: 4rem;
}
.vision .card {
    // padding: 1rem;
    padding: 1rem 2rem; // compensate for the text top bottom margin
    box-shadow: 0 2px 20px 0 rgba(0, 0, 0, 0.1);
    text-align: left;
    // margin-top: 2rem; // <-- you already have a gap between cards
    // border-radius: 1rem;
    background: #f3f0e8 url("/assets/img/icon_technologie1.svg") right -7rem center / 24rem
        no-repeat;

    &:nth-of-type(2) {
        background: #f3f0e8 url("/assets/img/icon_technologie2.svg") right -9rem center /
            28rem no-repeat;
    }

    &:last-of-type {
        // margin-bottom: 3rem;
        background: #f3f0e8 url("/assets/img/icon_technologie3.svg") right -7.8rem center /
            28rem no-repeat;
    }

    // .num {
    //     position: absolute;
    //     top: -2rem;
    //     left: 0.5rem;
    //     font-size: 4rem;
    //     font-weight: bold;
    //     opacity: 0.3;
    //     background: url('/assets/img/icon_technologie1.svg') center/cover no-repeat;
    //     width: 3.2rem;
    //     height: 3.2rem;
    // }
    strong {
        color: #ff5151;
        display: block;
    }
    p {
        font-size: 0.9rem;
        color: #000;
        overflow: hidden;
    }
}

// @media (max-width: 1199px) {
//     .top-area {
//         .inner {
//             &:before {
//                 width: 250px;
//                 height: 250px;
//             }
//         }
//     }
// }
// @media (max-width: 768px) {
//     .top-area {
//         padding-top: 12rem;

//         .inner {
//             &:before {
//                 content: none;
//             }
//         }
//     }
//     .wrap .content {
//         text-align: center;
//     }
// }
</style>
