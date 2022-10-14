<script>
import Pic from "../components/Pic.svelte"
import Card from "../components/Card.svelte"
import Section from "../components/Section.svelte"

const cardTitle1 = "Hello! My name is Christian"
const cardText1 = "Its a pleasure to meet you, I’m happy we could connect! If you’d like to add my contact information to your device you can tap the button below or you can keep scrolling to learn more about me and Igility Solutions..."
const cardCta1 = "Add to Contacts"

const sectionTitle1 = "Who am I?"
const sectionText1 = "Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Felis eget velit aliquet sagittis id. Habitant morbi tristique senectus et netus et malesuada. Purus non enim praesent elementum facilisis leo vel. Quam nulla porttitor massa id neque. Risus nullam eget felis eget nunc lobortis mattis. Ac tortor vitae purus faucibus ornare suspendisse sed nisi lacus. Ornare suspendisse sed nisi lacus sed viverra. Lacus sed turpis tincidunt id aliquet. In eu mi bibendum neque egestas congue quisque egestas. Orci nulla pellentesque dignissim enim sit amet. Metus aliquam eleifend mi in nulla posuere sollicitudin aliquam ultrices."

const sectionTitle2 = "Who is Igility Solutions?"
const sectionText2 = "Neque ornare aenean euismod elementum nisi quis eleifend quam adipiscing. Nisi scelerisque eu ultrices vitae. Elit ut aliquam purus sit amet luctus venenatis lectus magna. Mi sit amet mauris commodo quis. Malesuada proin libero nunc consequat interdum varius sit amet mattis. Cras semper auctor neque vitae tempus quam pellentesque nec. Pharetra et ultrices neque ornare. Morbi blandit cursus risus at ultrices mi. Lorem mollis aliquam ut porttitor leo a. Lectus arcu bibendum at varius vel pharetra. Pellentesque habitant morbi tristique senectus. Iaculis nunc sed augue lacus. Phasellus vestibulum lorem sed risus ultricies tristique. Nec dui nunc mattis enim ut tellus elementum sagittis vitae."

const cardTitle2 = "Curious to find out more?"
const cardText2 = "Then why not read more at our website:"
const cardCta2 = "IgilitySolutions.com"
</script>


<div class="w-full h-full fixed from-neutral-700 to-neutral-900 bg-gradient-to-br"></div>

<div class="fixed w-full h-screen">
    <ul class="pluses absolute top-0 left-0 w-full h-full overflow-hidden">
        <li><div class="vrt"></div><div class="hzt"></div></li>
        <li><div class="vrt"></div><div class="hzt"></div></li>
        <li><div class="vrt"></div><div class="hzt"></div></li>
        <li><div class="vrt"></div><div class="hzt"></div></li>
        <li><div class="vrt"></div><div class="hzt"></div></li>
        <li><div class="vrt"></div><div class="hzt"></div></li>
        <li><div class="vrt"></div><div class="hzt"></div></li>
        <li><div class="vrt"></div><div class="hzt"></div></li>
        <li><div class="vrt"></div><div class="hzt"></div></li>
        <li><div class="vrt"></div><div class="hzt"></div></li>
    </ul>
</div>

<div class="relative top-0 w-full h-full py-8 max-w-md m-auto flex flex-col items-center gap-y-5">

    <Pic />
    <Card title={cardTitle1} text={cardText1} ctaText={cardCta1} ctaLink={"#"} bgColor={"from-neutral-400/50 to-neutral-900/50 bg-gradient-to-br"} />
    <Section title={sectionTitle1} text={sectionText1} bgColor={"from-neutral-500/50 to-neutral-900/50 bg-gradient-to-br"} />
    <Section title={sectionTitle2} text={sectionText2} bgColor={"from-neutral-600/50 to-neutral-900/50 bg-gradient-to-br"} />
    <Card title={cardTitle2} text={cardText2} ctaText={cardCta2} ctaLink={"#"} bgColor={"bg-neutral-50/10"} classes={"text-center"} />

</div>


<style>

    .pluses li {
        position: absolute;
        display: block;
        list-style: none;
        width: 100px;
        height: 100px;
        animation: animate 25s linear infinite;
        top: -150px;
        opacity: 0.95;
    }

    .pluses li .vrt {
        border-radius: 4px;
        width: 35%;
        height: 100%;
        background-color: #3b82f6;
        margin: auto;
    }

    .pluses li .hzt {
        border-radius: 4px;
        width: 100%;
        height: 35%;
        background-color: #4ade80;
        position: relative;
        bottom: 68%;
    }

    .pluses li:nth-child(1){
        left: 25%;
        animation-delay: 10s;
    }


    .pluses li:nth-child(2){
        left: 10%;
        animation-delay: 2s;
        animation-duration: 12s;
    }

    .pluses li:nth-child(3){
        left: 45%;
        animation-delay: 26s;
    }

    .pluses li:nth-child(4){
        left: 20%;
        animation-delay: 2s;
        animation-duration: 18s;
    }

    .pluses li:nth-child(5){
        left: 65%;
        animation-delay: 0s;
    }

    .pluses li:nth-child(6){
        left: 40%;
        animation-delay: 32s;
    }

    .pluses li:nth-child(7){
        left: 35%;
        animation-delay: 14s;
    }

    .pluses li:nth-child(8){
        left: 50%;
        animation-delay: 15s;
        animation-duration: 45s;
    }

    .pluses li:nth-child(9){
        left: -10%;
        animation-delay: 8s;
        animation-duration: 35s;
    }

    .pluses li:nth-child(10){
        left: 75%;
        animation-delay: 8s;
        animation-duration: 11s;
    }

    @keyframes animate {

        0%{
            transform: translateY(0) rotate(0deg);

            border-radius: 0;
        }

        100%{
            transform: translateY(1000px) rotate(720deg);
            border-radius: 50%;
        }

    }


</style>
