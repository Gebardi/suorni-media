# Ohjeet ajastetuille ajoille (Radio Suorni, Instagram)

- Vastaa ja raportoi suomeksi.
- Julkaise Instagramiin vain `instagram-aikataulu.json`-rivejä, joilla `hyvaksytty` on true, `tila` on "odottaa" ja `pvm` on tänään (Europe/Helsinki). Ei koskaan muuta videota tai kuvatekstiä kuin rivillä.
- Julkaisu: vidIQ `vidiq_instagram_connected_accounts` → tili `radiosuorni` → `vidiq_video_upload` (url = rivin url) → `vidiq_instagram_publish_reel` (videoUrl = vidIQ:n palauttama, caption = rivin kuvateksti, ei isAiGenerated, ei trialParams). Jatka containerId/mcpJobId-kutsuilla kunnes PUBLISHED. Virheessä älä yritä uudelleen, raportoi.
- Päivitä rivin `tila` ("julkaistu"/"virhe") ja `permalink`, commit + push mainiin.
- Sanaa "Suno" tai Suno-tilin nimeä ei saa koskaan kirjoittaa julkiseen sisältöön.
