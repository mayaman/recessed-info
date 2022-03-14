<template>
  <div>
    <Announcement></Announcement>

    <header>
      <h1 class="cursive">Recessed</h1>
    </header>
    <Nav></Nav>
    <main>
      <div class="copy">
        <ul class="artists">
          <li class="artist">
            <div class="flex-left">
              <img
                class="artist-img"
                src="data:image/jpeg;base64,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"
                alt=""
              />
            </div>

            <div class="flex-right">
              <p>
                <span class="bold">Heidi Latsky’s</span> 38-year dance career
                began in Montreal, Canada, continued with Bill T. Jones/Arnie
                Zane Dance Company, and evolved further in 2001 when she founded
                her company, Heidi Latsky Dance (HLD). As New York’s largest
                physically-integrated dance company, HLD’s mission is to disrupt
                space, dismantle normal, and redefine beauty and virtuosity
                through innovative performance and discourse. Regarded by the
                New York Times as “a choreographer and dancer of uncommon
                intelligence and fluidity”, Latsky’s work has been featured at
                venues such as the American Dance Festival, Joyce Theater, High
                Line, National Portrait Gallery, The Whitney Museum, and Lincoln
                Center for the Performing Arts. Her work GIMP was nominated for
                an Emmy, and her artistic portfolio has been supported by
                Creative Capital, The MAP Fund, Ford Foundation, National
                Endowment for the Arts, Canada Council for the Arts, and New
                York State Council on the Arts, among others. Most recently,
                Latsky received the Martha Hill Dance Fund Mid-Career Award.
              </p>
              <br />

              <p>
                <a target="_blank" href="https://heidilatskydance.org/"
                  >heidilatskydance.org</a
                >
              </p>
            </div>
          </li>

          <li class="artist">
            <div class="flex-left">
              <img
                class="artist-img"
                src="https://storage.googleapis.com/recessed-assets/maya/me.jpg"
                alt=""
              />
            </div>

            <div class="flex-right">
              <p>
                <span class="bold">Maya Man</span> (she/her) is an artist,
                programmer, and dancer. Her work considers the computer screen a
                space for intimacy and performance, focusing on the phenomenon
                of translating our offline selves into on-screen content. She
                spends most of her time creating work for the world wide web,
                dancing in studios and public spaces, and maintaining her
                love/hate relationship with the Internet (mostly love though).
                She holds Bachelor of Arts degrees in Computer Science and Media
                Studies from Pomona College. She is currently pursuing an MFA in
                Media Arts UCLA in Los Angeles.
              </p>
              <br />
              <p>
                <a target="_blank" href="https://mayaontheinter.net/"
                  >mayaontheinter.net</a
                >
              </p>
            </div>
          </li>

          <li class="artist">
            <div class="flex-left">
              <img
                class="artist-img"
                src="https://storage.googleapis.com/recessed-assets/sabrina/image/02.jpg"
                alt="Black and white image of Sabrina performing in a white costume"
              />
            </div>

            <div class="flex-right">
              <p>
                <span class="bold">Sabrina Bennett</span>
                is a 35 year old artist born from Jamaican Immigrants. As an L1
                incomplete paraplegic, Sabrina has turned trauma into triumph.
                She is a peer mentor for other individuals with spinal cord
                injuries, an adaptive Zumba instructor for senior citizens, and
                a model - spreading awareness about the importance of adaptive
                clothing. Dancing since a young age, Sabrina has performed
                ballroom dancing with Roll Call, and contemporary dance with ZCO
                Dance Company and Heidi Latsky Dance. During her time with HLD,
                Sabrina has been challenged to use raw emotion and translate it
                into movement, which has been a powerful experience.
              </p>
            </div>
          </li>

          <li class="artist">
            <div class="flex-left">
              <img
                class="artist-img"
                src="https://storage.googleapis.com/recessed-assets/desmond/image/04.jpg"
                alt="Black and white image of Desmond performing with his face to the sky"
              />
            </div>

            <div class="flex-right">
              <p>
                <span class="bold">Desmond Cadogan</span> initially started his
                dance training at Les Ballet Jazz de Montreal and continued at
                the Dance Theater of Harlem School and Joffrey Ballet School.
                His time at the Royal Winnipeg Ballet School left Cadogan
                terribly injured making it difficult for him to start a
                performing career early in life. After modeling for many years,
                Desmond took classes from Heidi Latsky in Canada. When he
                observed an HLD rehearsal, it was love at first sight. After
                years of modeling for artists like Robert Mapplethorpe, Jean
                Michel Basquiat, and Rainer Fetting, with whom Desmond sat for
                many paintings and sculptures, "ON DISPLAY" felt like a perfect
                fit. It has been a dream come true and tremendous honor for him
                to dance with HLD for the last four years.
              </p>
            </div>
          </li>

          <li class="artist">
            <div class="flex-left">
              <img
                class="artist-img"
                src="https://storage.googleapis.com/recessed-assets/meredith/image/MeredithFagesbyAnnette%20Kolzow-4.jpg"
                alt="Black and white image of Meredith performing in a white costume"
              />
            </div>

            <div class="flex-right">
              <p>
                <span class="bold">Meredith Fages</span> joined HLD in 2007 and
                has also performed with Motley Dance, Steeledance, Jimena Paz,
                Laura Peterson, Todd Rosenlieb Dance, and Virginia Ballet
                Theatre, featured in Ashton, Balanchine, Christensen, Tudor
                ballets. Described by Deborah Jowitt as a “remarkable
                dancer...adept in some society of the future, [a] primal,
                near-aquatic creature slipping around in a watery world...”, she
                graduated from Columbia University with a Pre-Medical
                Concentration in English. Her writing has appeared in Dance
                Magazine and Dance Teacher.
              </p>
            </div>
          </li>

          <li class="artist">
            <div class="flex-left">
              <img
                class="artist-img"
                src="https://storage.googleapis.com/recessed-assets/jillian/image/01.jpg"
                alt="Black and white image of Jillian performing in a white costume"
              />
            </div>

            <div class="flex-right">
              <p>
                <span class="bold">Jillian Hollis</span>, originally from
                Syracuse, NY, is a Point Park University graduate who joined HLD
                in 2002 and is now the company's Rehearsal Director. Her dancing
                has been described as “blithely irrepressible” by The NY Times.
                In addition to Jillian’s work with Heidi Latsky Dance, she
                collaborates with other artists, is a burlesque performer, and
                was Miss Coney Island 2018.
              </p>
            </div>
          </li>

          <li class="artist">
            <div class="flex-left">
              <img
                class="artist-img"
                src="https://storage.googleapis.com/recessed-assets/donald/image/02.jpg"
                alt="Black and white image of Claude performing in a white costume"
              />
            </div>

            <div class="flex-right">
              <p>
                <span class="bold">Donald Lee</span> is a disabled artist based
                in New York City and an HLD company member. In his transgressive
                artistic practice, he prides amateurism as an approach to create
                varied work that challenges and delights all audiences,
                provoking questions about conventions in aesthetics structures.
                He is process-oriented and advocates for disability artistry and
                inclusivity in the arts for which he has been quoted by ARTNews,
                Fjord Review, and The New York Times. He has performed with HLD
                at the United Nations, Whitney Museum, National Portrait
                Gallery, and at City Winery as part of Perry Farrell’s Kind
                Heaven Orchestra Tour.
              </p>
            </div>
          </li>

          <li class="artist">
            <div class="flex-left">
              <img
                class="artist-img"
                src="https://storage.googleapis.com/recessed-assets/claude/image/01.jpg"
                alt="Black and white image of Claude performing in a white costume"
              />
            </div>

            <div class="flex-right">
              <p>
                <span class="bold">Claude Andrée Louissaint</span> has an M.A.
                from NYU in Performing Arts Administration, and has worked at
                Danspace Project, Orpheus Chamber Orchestra, and American
                Symphony Orchestra. Claude has been working with Heidi and her
                company since 2001.
              </p>
            </div>
          </li>

          <li class="artist">
            <div class="flex-left">
              <img
                class="artist-img"
                src="https://storage.googleapis.com/recessed-assets/sora/image/02.jpg"
                alt="Black and white image of Claude performing in a white costume"
              />
            </div>

            <div class="flex-right">
              <p>
                <span class="bold">Sora Sol</span> is the Co-Founder,
                Entertainment Director, and Head Diva of CirqOvation. In 2013,
                she founded CirqOvation with her husband, Josh, and started
                gathering a team of incredibly talented, kind, quirky humans who
                now make up their performing family. Sora is proudly
                Japanese-American, Queer, Disabled/disfigured. In addition to
                being a circus artist and producer, she is a writer who is
                passionate about envisioning empathic paths towards equity. Sora
                began working with Heidi on a film featuring herself during the
                pandemic. The film premiered at the Astoria Performing Arts
                Center in Long Island City July 2021.
              </p>
            </div>
          </li>
        </ul>
      </div>
    </main>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
::selection {
  color: white;
  background: #6289fb;
}

ul.artists {
  list-style: none;
  margin-top: 0px;
  padding-top: 0px;
  padding: 0px;
  margin: 0px;
}

/* li.artist {
  display: flex;
  align-items: top;
  margin: 50px auto;
  max-width: 100%;
}; */

li {
  margin: 0 auto 100px auto;
  display: flex;
  justify-content: space-between;
}

.flex-left {
  width: 30%;
}

.flex-right {
  padding-left: 50px;
  width: 70%;
}

p {
  margin: 0px;
}

.artist-img {
  width: 100%;
  margin: auto;
  display: block;
}
</style>