<header class="sticky-header">
	<p class="header-text">portfolio | rou-kay-uh-too fey</p>
	<ul class="header-links">
		<li><a href="#about">about</a></li>
		<li><a href="#works">works</a></li>
        <li><a href="#contact">info</a></li>

	</ul>
</header>

<div class="name-block">
	<div class="name">
		<h1 class="first">ROKHEYATOU</h1>
		<h1 class="last">FAYE</h1>
	</div>

	<div class="portrait">
		<img
			src="https://instagram.ftpa1-2.fna.fbcdn.net/v/t51.82787-15/541554003_18374507185179942_9073538595774707118_n.jpg?stp=dst-jpg_e35_tt6&_nc_cat=102&ig_cache_key=MzcxMjM1MjQyNjg0MzU4MTY4OA%3D%3D.3-ccb7-5&ccb=7-5&_nc_sid=58cdad&efg=eyJ2ZW5jb2RlX3RhZyI6InhwaWRzLjE0NDB4MTkwNS5zZHIuQzMifQ%3D%3D&_nc_ohc=xZ2n3IzC8q8Q7kNvwFexNCi&_nc_oc=Adl9cseExYoaAb2ojuZzkbnmu5Rk5x4KFrduCsVAW8SCQhbtoVIyyZ2tZp3lT3t8Y-FbjSVWpNwYw7fR25fQjUIy&_nc_ad=z-m&_nc_cid=0&_nc_zt=23&_nc_ht=instagram.ftpa1-2.fna&_nc_gid=wuMTJyGzfO1cq8dIbCk1zA&oh=00_AfofGu0AhpjfSfyvMldF4rYbQlpITJy-ZLmoIBvTQz6QFA&oe=69610882"
			width="100%"
			alt="portrait of artist"
		/>
	</div>
</div>

<div id="about" class="about-me-block">
	<p>
		My name is Rokheyatou Faye. I am a mechanical engineer and visual artist working at the
		intersection of design, visual systems, and storytelling.

		<br /> <br />

		My practice moves between systems-driven thinking and creative intuition that is shaped by a
		background in engineering, studio art, and cultural institutions.

		<br /> <br />

		I build, question, prototype, and refine through an exploration of the material world to examine
		how form, function, and meaning coexist.
	</p>
</div>

<div id="works" class="works-block">
    <p>
        yadada
    </p>
</div>

<style>
	.sticky-header {
		position: static;
		top: 0;
		display: flex;
		align-items: center;
		justify-content: space-between;

		padding-inline: clamp(0.5rem, 4vw, 3rem);
		gap: clamp(1rem, 6vw, 4rem);

		font-size: clamp(0.25rem, 3vw, 2rem);
		height: clamp(0.5rem, 10vh, 7rem);

		font-family: 'Google Sans', sans-serif;
		font-weight: 600;
		/* overflow: hidden; */
	}

	.header-text {
		white-space: nowrap;
		line-height: 1;
		color: white;
	}

	.header-links {
		display: flex;
		gap: clamp(0.5rem, 3vw, 2rem);
		list-style: none;
		margin: 0;
		padding: 0;
	}

	.header-links li a {
		color: white;
		text-decoration: none;
		white-space: nowrap;
		font-size: inherit;
		/* FIX 1: Provide a reference point for the absolute underline */
		position: relative;
		display: inline-block; /* Helps with alignment and padding */
	}

	.header-links li a::after {
		content: '';
		position: absolute;
		left: 0;
		/* FIX 2: Bring it closer so overflow:hidden doesn't cut it off, 
       or adjust the header height/padding */
		bottom: -4px;
		width: 100%;
		height: 4px;
		background-color: white;
		transform: scaleX(0);
		transform-origin: bottom left;
		transition: transform 0.25s ease-in-out; /* Slowed down slightly for better visibility */
	}

	.header-links li a:hover::after {
		transform: scaleX(1);
		transform-origin: bottom left;
	}

	.header-links li a:visited {
		text-decoration: none;
		color: white;
	}

	.name-block {
		display: block;
		background-color: #818c7e;
		position: static;
		inset: 0;
		height: fit-content;
		overflow-x: hidden;
		overflow-y: hidden;
	}

	.name {
		display: block;
		position: relative;
		font-family: 'Instrument Serif';
		color: #a74d4a;
		z-index: 1;
		left: 2%;
	}

	.first {
		font-size: 17vw;
		margin-top: 0;
		margin-bottom: 0;
		line-height: 0.9;
	}

	.last {
		font-size: 28vw;
		margin-top: 0;
		margin-bottom: 0;
		line-height: 1;
	}

	.portrait {
		position: absolute;
		z-index: 0;
		/* border: 5px solid pink; */
		width: 40%;
		left: 55%;
		top: clamp(5.5rem, 12vw, 10rem);
	}

	.about-me-block {
		position: relative;
		margin-top: 300px;
		font-family: 'Google Sans', sans-serif;

		/* border: 3px solid red; */

		left: 2%;
		width: 65%;
		font-size: xx-large;
		font-weight: 600;
		color: white;
	}
</style>
