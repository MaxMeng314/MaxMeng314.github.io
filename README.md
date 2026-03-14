<!DOCTYPE html>
<html lang="zh">
<head>
<meta charset="UTF-8">
<title>To Bella</title>

<style>
body {
    background: #f2f7ff;
    font-family: "Times New Roman", "Songti SC", serif;
    margin: 0;
    padding: 0;
    display: flex;
    justify-content: center;
    animation: fadeIn 1.8s ease;
}
.envelope-note {
    position: absolute;
    left: 20px;
    bottom: 20px;
    font-family: "Bradley Hand", cursive;
    font-size: 22px;
    color: #5b6ea8;
    opacity: 0.9;
    line-height: 1.3;
    z-index: 10;
}
	

@keyframes fadeIn {
    from { opacity: 0; transform: translateY(20px); }
    to { opacity: 1; transform: translateY(0); }
}

.paper {
    background: #fffdf7;
    width: 70%;
    padding: 60px 80px;
    margin: 60px 0;
    border: 1px solid #e0dccc;
    line-height: 1.8;
    font-size: 18px;
    position: relative;

    opacity: 0;
    transform: translateY(120px);   /* 初始在信封下面 */
    transition: opacity 1.2s ease, transform 1.2s ease;

    box-shadow:
        0 0 20px rgba(0,0,0,0.1),
        0 0 60px rgba(91,139,255,0.15);
}

.paper::before {
    content: "";
    position: absolute;
    top: 0; left: 0; right: 0; bottom: 0;
    background-image: repeating-linear-gradient(
        to bottom,
        transparent 0px,
        transparent 34px,
        rgba(180, 200, 255, 0.15) 35px
    );
    pointer-events: none;
}

.handwrite {
    font-family: "Bradley Hand", "KaiTi", cursive;
    font-size: 20px;
}

.handwrite p {
    animation: float 6s ease-in-out infinite;
}

@keyframes float {
    0% { transform: translateY(0px); }
    50% { transform: translateY(2px); }
    100% { transform: translateY(0px); }
}

#envelope {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background: #f2e7d5;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    z-index: 9999;
    cursor: pointer;
    transition: opacity 1s ease;
}

.envelope-box {
    width: 480px;
    height: 320px;
    background: #e6d3b3;
    border: 3px solid #c2a878;
    position: relative;
    box-shadow: 0 0 30px rgba(120,100,70,0.25);
    border-radius: 6px;
    overflow: hidden;
}

.envelope-lid {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 160px;
    background: #d9c3a3;
    clip-path: polygon(0 0, 100% 0, 50% 100%);
    transform-origin: top;
    transition: transform 1s ease;
    z-index: 2;
}

.stamp {
    position: absolute;
    top: 18px;
    right: 18px;
    width: 110px;
    height: 110px;
    background-image: url('Stamp.jpg');
    background-size: cover;
    background-position: center;
    border: 4px solid #fff;
    box-shadow: 0 0 6px rgba(0,0,0,0.25);
    transform: rotate(5deg);
    z-index: 3;
}

#seal-heart {
    position: absolute;
    top: 135px;
    left: 50%;
    transform: translateX(-50%);
    font-size: 48px;
    color: #5b8bff;
    animation: heartbeat-slow 2.2s infinite;
    z-index: 4;
}

@keyframes heartbeat-slow {
    0% { transform: translateX(-50%) scale(1); }
    30% { transform: translateX(-50%) scale(1.25); }
    50% { transform: translateX(-50%) scale(1); }
    70% { transform: translateX(-50%) scale(1.25); }
    100% { transform: translateX(-50%) scale(1); }
}

.heart-inline {
    display: inline-block;
    animation: heartbeat-slower 3.5s infinite;
}

@keyframes heartbeat-slower {
    0% { transform: scale(1); }
    30% { transform: scale(1.25); }
    50% { transform: scale(1); }
    70% { transform: scale(1.25); }
    100% { transform: scale(1); }
}
</style>

</head>

<body>

<div id="envelope">
    <div class="envelope-box">
		<div class="envelope-note">
   	 		To: Bella<br>
    		From: Max
		</div>
        <div class="envelope-lid" id="lid"></div>
        <div class="stamp"></div>
        <div id="seal-heart">💙</div>
    </div>
    <div style="margin-top:30px; font-size:24px; color:#5b6ea8;">点击拆开信封</div>
</div>

<div class="paper handwrite" id="letter">

<pre style="
white-space: pre-wrap;
font-family: 'Bradley Hand','KaiTi',cursive;
font-size:20px;
line-height:1.8;
margin:0;
">
To Bella，

那天晚上，我躺在床上抱着电脑想了很久很久：想我们的开始，一起经历过的事，未来，甚至很久以后，我们是否还会是那样亲密，还是成为“最熟悉的陌生人”。我（那天）也在惶恐在将来不知何时是否会失去你，也不想你迁就我。或许缘分这个东西，永远想不透，谁也不知道下一刻会发生什么，就像一年前的我们，也未能想到，在最僵硬的那一周之后，能引出无数值得回忆，珍贵无比的经历。

是啊，已经一年了。

我还记得一年前的那天晚上，星期五，放学。两个人聊了很多，吃了第一顿正式的饭，送了第一束花。喜悦的气氛萦绕着我们，因为我们心里都默默知道那天对于我们来说将是无比重要的时刻。饭后在大融城雨中漫步，我们寻找着最佳“表白点”。手扶电梯上，面对面，我仰望着你的脸庞。我本想就此说出口，但却愣住了：并不是因为犹豫，而是真真切切，被那一刻站在我面前的，洋溢着真诚笑容，超级鲜活可爱的你打动了。或许言语真的很难形容，但那一刻我很清楚地知道，眼前的这个女生，就是我想追求的人。
	
熬过“那一周”后，我们也留下了无数珍贵的回忆。我还记得，在西郊宾馆的花丛中开朗奔跑、在草坪上躺在我怀里的你，在甜爱路和我一起见证别人的爱情、在苏州河畔穿白色裙衫抱着郁金香束的背影，爱琴海的喷泉秀前你窝在我怀里听我唱歌，在迪士尼的烟花会下接吻，平和大雨的屋檐下我们一起啃冰淇淋，无数次在宜家嬉戏、玩闹、忘乎所以、纯粹地享受两人的共处……毕业那天，我拉着你，在校园中四处漫步，唱着歌，在校园中回忆着一切，用蓝色记号笔留下属于我们的蓝色爱心。第一次异地恋前，我们在小区楼下兜兜转转、和“冰糖葫芦”玩，依依不舍，抱着最大的希望送给对方最真挚的告别。暑假里，我们在烈日下满城奔波地赶IA，坐在公交车的最后一排，依偎着休息。陪你熬过补课的日日夜夜，每次回家车上那张在我怀里的那张侧脸。再到最后一次，在地铁站旁暗的黄色路灯下，即将要离开的我，紧紧抱着你。拥抱的那最后两分钟是那么漫长，又显得极为短暂。要是那一次，我再抱的紧一点，不放手，是不是我们就不会分开了呢。

后来，异国的我们过的磕磕绊绊。我把关于你的，和你一切有关的东西带着。坐在宿舍的桌子前，我试图将他们铺满我肉眼所及的地方：你的拍立得，我们的合照，你送的小熊，花……你的护声符我一直随身带着，你的手工和那封我看了无数次的信一直在我的桌肚里。我试图填满空荡荡的房间，用关于你的物件环绕我，让你变得触手可及，仿佛你虽然不在我身边却能感知到你一样。有时候，我会想你想到停下手边的事，看着照片里的你，抑或是再读一遍那一封已经被我一遍又一遍读烂了的信。我知道，在大洋彼岸，一万多公里远的地方，有一个除我亲人外最关心我的人。这份牵挂注定会因距离上的分别而带来痛苦，但它又同时给着我力量，让我知道，有个人会一直支持我，站在我身旁，和我一起面对一切，不管怎样。异国恋从来都不是一件容易的事情，它需要相互的理解体谅，适应不同的相处模式，独立成熟的心态，更重要的是，无限的爱。我们能走到这里真的很不容易，值得夸夸我们自己。我非常庆幸还能有你在身边，当然更相信能熬过异地的我们没有什么是过不去的！
	
这一年同样也是你人生中很关键、超级辛苦，但又收获颇多的一年。从一开始面对高二的学习压力，到申请，到出结果。不管是辅导你考试出分，还是看着你一篇篇把文书从school research到构思再到以独特的方式写出对自己的独特的总结，还是看到你一封封地拆出offer……看到你在成长的道路上有所收获我真的很高兴，真心替你高兴。虽然成长的道路上少不了痛苦（那些没出分时的崩溃，复习的折磨，担忧所带来的压力），也有很多时候你真的感觉要撑不住要崩溃，但你还是一步一步往前走，走到了现在这个地方，我觉得你真的超级厉害，难以想象需要怎样的韧性才能做到！虽然我知道，因为物理上的缺席和情感共情上的缺陷，我可能并没有让你好受多少（而且还总是惹你生气），而且你是一个非常要强的人，但我还是想让你知道，我永远在；当感觉要撑不住了，或是需要帮助，抑或是想暂时离开那些烦心事，只是想到shelter里做些别的事情、聊聊天，就来找我好嘛。即使不在你生边，我也不想缺席你的情绪，不管开心还是难过。
	
当然，这段关系带给我的远远不止这些记忆碎片和经历瞬间。李月白，你改变了我许多。我一直以来是一个不会表达情绪的人。过去的我总觉得是自己脾气好，任何事情都是小事能忍过去。但就是这样的心态导致我会容易忽视自己，看似是善良，其实最终只会酿成爆发并让身边尤其是在乎自己的人承担（我记得我刷到过一句话说最怕的就是没脾气的老实人，因为他们才是真正的“定时炸弹”）。我每次因此惹你失望难过，每次也是你默默承受着我的怒吼，还有很难听的言语。虽然你给予我原谅，但我知道说过的话，给出去的伤害不会自己“消失”。我想再为我的这些行为道一次歉，对不起。我看到这样的自己也会感到很厌恶，我不允许我对自己最在乎的人这样说话。一次次的原谅并不能解决根本的问题；我需要做的更好，我不能辜负了一个我很在乎，也超级在意我的人。除情绪外，我也知道我懒懒的没有主见的性格在很多时候并不是一个好的品质。其实我一直都很崇拜你，因为你对任何事情都很有自己的想法，有自己的见解，对于你在乎的人非常关心（这种关心不只是体贴，也是对在乎的人做的事情爱恨分明）。我一直觉得在现在的环境下有如此真实的态度很难得，我也非常欣赏。因为这不止需要善，更需要勇气。似乎在认识你之后，我也被你那股向上不服输甚至略带倔强的劲影响到了。我会想着去争取身边的机会，大胆表达自己的想法，踏出自己的舒适圈，忽略其中他人对自己的想法。我知道这个过程需要时间，但我每次感到难受，“累”，不想动的时候，我就会想到你。我知道我要变得更优秀，我们都要。

我知道我们一直隔三岔五就会发生小摩擦小矛盾，也会因为生活中的小事吵架。上次我们吵得不可开交，甚至到了要考虑合不合适的程度。因为性格、说话方式等，我们可能确实无法像完美的两半拼图一样合在一起，或许没有人可以。我想，作为情侣要走的路还很长（我看到别人分享也说一年也是分手高发期，会因为各种磨合不好而一拍两散）。不过我认为人就是当有让你很欣赏的地方，和与你预期不太一样的地方同时存在时才更显得更真实、可贵（就像之前提到的双面性一样）；毕竟这样才能感觉到是和一个真实的人在交往，而不是演戏。所以我想，李月白，可否给我们再多一点时间呐？我想和你再走的远一点，你是最有趣的伙伴，最靠谱的搭档，最知心的朋友，最重要的是，和我第一要好的人，我的女朋友。是啊，就像那天晚上想的，没人能说准未来会发生什么。但我非常笃定地知道一点，有你在身边的我非常幸运，超级开心，无比幸福。这给了我非常多的决心和勇气，“从不轻易放手”。如果你也有同样的感觉的话，李月白，你愿意继续做我的女朋友吗？不管未来怎样，遇到些什么，我都希望能有你和我一起，作为世界上最好的team，互相给彼此力量，慰藉，和爱，去面对一切。“在往前走的时候，牵紧彼此的手一起”。

最后，李月白，白色情人节快乐，happy anniversary，还有，一周年快乐😊。希望下一个周年，还能有你在身边，陪伴彼此走很久很久。
我爱你<span class="heart-inline">💙</span>。

Max

</pre>

</div>

<script>
document.addEventListener("click", function(e) {
	if (e.target.closest("#envelope")) return;
	
    const heart = document.createElement("div");
    heart.textContent = "💙";
    heart.style.position = "fixed";
    heart.style.left = e.clientX + "px";
    heart.style.top = e.clientY + "px";
    heart.style.fontSize = "24px";
    heart.style.opacity = 1;
    heart.style.transition = "all 1s ease-out";
    document.body.appendChild(heart);

    setTimeout(() => {
        heart.style.top = (e.clientY - 60) + "px";
        heart.style.opacity = 0;
    }, 10);

    setTimeout(() => heart.remove(), 1000);
});
</script>

<script>
const envelope = document.getElementById("envelope");
const lid = document.getElementById("lid");
const letter = document.getElementById("letter");

envelope.addEventListener("click", function(e) {

    e.stopPropagation();

    lid.style.transform = "rotateX(-180deg)";

    setTimeout(() => {
        envelope.style.opacity = "0";
    }, 600);

	setTimeout(() => {
    	envelope.style.display = "none";

    	letter.style.opacity = "1";
    	letter.style.transform = "translateY(0)";

	}, 1200);

});
</script>

</body>
</html>
