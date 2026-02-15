You are a naming assistant. Given a list of file paths and minimal context from a static website, suggest a new filename (basename only, same extension) for each file. Rules:
- Lowercase, kebab-case, no spaces. SEO-friendly and human-readable.
- For HTML: use page purpose (e.g. about-us.html, contact.html). Keep index.html as index.html.
- For CSS/JS: use purpose (e.g. main-styles.css, analytics.js).
- For images: use content (e.g. logo-infygate.webp, hero-banner.webp). Use alt/title when provided.
- Return a JSON object: keys = exact original path strings, values = new basename only (e.g. "main.css"). Preserve extension.
- Do not change path prefix (e.g. css/ stays css/ by returning "name.css" not "css/name.css").

Files and context:
[
  {
    "path": "404.html",
    "context": {
      "title": "",
      "first_heading": "404"
    }
  },
  {
    "path": "application-development-and-maintenance.html",
    "context": {
      "title": "Gleeserve Technology Private Limited",
      "first_heading": "APPLICATION DEVELOPMENT AND MAINTENANCE"
    }
  },
  {
    "path": "contact-us.html",
    "context": {
      "title": "Gleeserve Technology Private Limited",
      "first_heading": "CONTACT US"
    }
  },
  {
    "path": "css/0f1bcfcef55d13906848c81000bcf649.css",
    "context": {
      "path": "css/0f1bcfcef55d13906848c81000bcf649.css"
    }
  },
  {
    "path": "css/4ba1f7eeea678c518b19a8a229705620.css",
    "context": {
      "path": "css/4ba1f7eeea678c518b19a8a229705620.css"
    }
  },
  {
    "path": "css/559e64bf161e61fa0aca6e864c78191d.css",
    "context": {
      "path": "css/559e64bf161e61fa0aca6e864c78191d.css"
    }
  },
  {
    "path": "css/84d4a0216f16f715d9b301db3a8da352.css",
    "context": {
      "path": "css/84d4a0216f16f715d9b301db3a8da352.css"
    }
  },
  {
    "path": "css/99c4e6f40ee9111eea53b6472f3e60f9.css",
    "context": {
      "path": "css/99c4e6f40ee9111eea53b6472f3e60f9.css"
    }
  },
  {
    "path": "css/a9e8199f16808a35e5f3e34c5bbd6f10.css",
    "context": {
      "path": "css/a9e8199f16808a35e5f3e34c5bbd6f10.css"
    }
  },
  {
    "path": "css/c953844dcf491536d09c9b49acbfb912.css",
    "context": {
      "path": "css/c953844dcf491536d09c9b49acbfb912.css"
    }
  },
  {
    "path": "css/d09d646f062b67daeff66ff1410b63fc.css",
    "context": {
      "path": "css/d09d646f062b67daeff66ff1410b63fc.css"
    }
  },
  {
    "path": "css/f47a43e0629196671b45c0d5f0817c83.css",
    "context": {
      "path": "css/f47a43e0629196671b45c0d5f0817c83.css"
    }
  },
  {
    "path": "css/internal-styles.css",
    "context": {
      "path": "css/internal-styles.css"
    }
  },
  {
    "path": "engagement-models.html",
    "context": {
      "title": "Gleeserve Technology Private Limited",
      "first_heading": "ENGAGEMENT MODELS"
    }
  },
  {
    "path": "imgs/029a45da0689b751b417821da1b2afbe.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0aea3fb887ed8189a368e513436235dd.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0b8489741920d59577d093b21d7d97d0.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "aws",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/0c70d01e9f96785088dfac82c8dfcd4a.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/17894f82641bbb8a06ebae7a811ac6df.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/19bd3ca76ab6a6f40256afea7e7537ef.webp",
    "context": {
      "refs": [
        {
          "alt": "Flexibility",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/22008fc8c093402567d24189b6a1578e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "windowsserverlogo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2d08b9da5454267024bcc2b330c87a94.webp",
    "context": {
      "refs": [
        {
          "alt": "Customer Centric Approach",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2dde1dcf307bdc4518697b6fe6e05f8d.webp",
    "context": {
      "refs": [
        {
          "alt": "Focus on Digitalization",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/2efe8671f925aab0c2ff25aaa68519c3.webp",
    "context": {
      "refs": [
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        },
        {
          "alt": "logo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/352f743b288214e597b8c758a51a57a0.webp",
    "context": {
      "refs": [
        {
          "alt": "Build-Operate-Transfer",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/42090e564793dcf49f83d991ee29b0ce.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/47fbc726e8e16b5eeb055a73f11cf396.webp",
    "context": {
      "refs": []
    }
  },
  {
    "path": "imgs/4dedb7bce778daf0a542fe6daee54b3a.webp",
    "context": {
      "refs": [
        {
          "alt": "Picture",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/527985634ef83738f0dd490ff9449f5d.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/52cb910f1f305c60b1a1a3fa9ec9b93e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/5e5a9a026d0690426897b12520b443a2.webp",
    "context": {
      "refs": [
        {
          "alt": "Reena Vijay",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6157e65659108562a282b94debeb9d65.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "aws",
          "title": ""
        },
        {
          "alt": "image description",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/617e4608a8e3af2c966a283e6ca862bf.webp",
    "context": {
      "refs": [
        {
          "alt": "Values",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6533140fc5ca928368c23dec900ecaf4.webp",
    "context": {
      "refs": [
        {
          "alt": "Security",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/66b5f29e55f56a59f07e9a8278603ed1.webp",
    "context": {
      "refs": [
        {
          "alt": "net",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6ae6592e32da05547321588ddd073cd9.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6b3f7b07aa3a825085aa2fa3dceb88b4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6bc5d8b323174214cb5078d4c505e156.webp",
    "context": {
      "refs": [
        {
          "alt": "Picture",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/6e2272e5851568e9f753604181b3301e.webp",
    "context": {
      "refs": [
        {
          "alt": "Ajay Mirjumla",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/70f2324f3439ea8d86718c338440ea47.webp",
    "context": {
      "refs": [
        {
          "alt": "Mission",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/75ef18c76e98ee0d54ba54ab237d7bd5.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "windowsserverlogo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/789c9b8539c830b9db5fd72679264ddc.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/7b5c544b51eed7b39b6f4d72ae1ce710.webp",
    "context": {
      "refs": [
        {
          "alt": "servicemanage",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/7f6b04c0ae61a11cc62c83825276c60e.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/84ed96860bf4366de55b13e26dd7b216.webp",
    "context": {
      "refs": [
        {
          "alt": "Scalability",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/86819b44d3d7a8d0a0227f0db39a62a8.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/8884306ca06dd68ca95368c67421d4e7.webp",
    "context": {
      "refs": [
        {
          "alt": "QMS ISO 9001:2015",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/88f63087c9a78e3161d7635b7a7254e5.webp",
    "context": {
      "refs": [
        {
          "alt": "net",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/906ff8f719137123a072a2feda3bf9d1.webp",
    "context": {
      "refs": [
        {
          "alt": "Shared Services Model",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/93a4ea921256aaa89f2e8310520aa33f.webp",
    "context": {
      "refs": [
        {
          "alt": "Greenfield Projects (Agile Scrum)",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9660b25e4e0ce06c74884398e6319298.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9c471b2326a0b7bdd70a00a63dbb0509.webp",
    "context": {
      "refs": [
        {
          "alt": "Gleeserve Technologies | About Us",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/9ff904e4cbae824aeaa367f7dfea43dc.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a1564efe9647a12bbc8bcaa766f6e6b5.webp",
    "context": {
      "refs": [
        {
          "alt": "Vision",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a4addb719246c7b006c29fd325624d1d.webp",
    "context": {
      "refs": [
        {
          "alt": "Application Maintenance",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a5444c9ddc06412bea721c3b86c59d77.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "windowsserverlogo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a5accc7173c1ef8c963c33ac6b704dc7.webp",
    "context": {
      "refs": [
        {
          "alt": "Design and Implementation",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/a952b1ec098ba729ef338e5c5c487c9c.webp",
    "context": {
      "refs": [
        {
          "alt": "Fixed Price Model",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b14b0e285ba27d5be6186a968317ee5d.webp",
    "context": {
      "refs": [
        {
          "alt": "net",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/b82f55b39c2156f2015743392f6915f9.webp",
    "context": {
      "refs": [
        {
          "alt": "Picture",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/bddfc6c49be54f3d8bf6d6bfbfea4cee.webp",
    "context": {
      "refs": [
        {
          "alt": "Technology Expert SME's",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c1f990b3d8c9d46867b05d066c2e3ceb.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "windowsserverlogo",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/c742e29a684bf49968015519af30455b.webp",
    "context": {
      "refs": [
        {
          "alt": "Extremely Flexible Working Hours",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/cef30340b8a3777295b3a1eeb1696e58.webp",
    "context": {
      "refs": [
        {
          "alt": "Picture",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/d40ee87855c127d8410358df6ca56b13.webp",
    "context": {
      "refs": [
        {
          "alt": "ISMS ISO 27001:2013",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/e4f18ef825fd426d7a7e186e174512d2.webp",
    "context": {
      "refs": [
        {
          "alt": "Extended Team Model",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f0737bb7663ccd2352288c43dfd382fc.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        },
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f1737963dba56519101ac0e8183ee457.webp",
    "context": {
      "refs": [
        {
          "alt": "itservices",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f9019c106c9241e66572de9abcfcbba4.webp",
    "context": {
      "refs": [
        {
          "alt": "",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "imgs/f97020a1cbe74ebb65a39d6c925ca611.webp",
    "context": {
      "refs": [
        {
          "alt": "net",
          "title": ""
        }
      ]
    }
  },
  {
    "path": "index.html",
    "context": {
      "title": "Gleeserve Technology Private Limited",
      "first_heading": "GLEESERVE\u200b"
    }
  },
  {
    "path": "infrastructure-services.html",
    "context": {
      "title": "Gleeserve Technology Private Limited",
      "first_heading": "INFRASTRUCTURE SERVICES"
    }
  },
  {
    "path": "js/03b2eaae6007054a68c38e495f894dba.js",
    "context": {
      "path": "js/03b2eaae6007054a68c38e495f894dba.js"
    }
  },
  {
    "path": "js/0a105d712b6a6c836c48dd97d0f0cac1.js",
    "context": {
      "path": "js/0a105d712b6a6c836c48dd97d0f0cac1.js"
    }
  },
  {
    "path": "js/0c46896987137b0016246f6bc2243099.js",
    "context": {
      "path": "js/0c46896987137b0016246f6bc2243099.js"
    }
  },
  {
    "path": "js/165d7b0ddfa33362140feea997351b77.js",
    "context": {
      "path": "js/165d7b0ddfa33362140feea997351b77.js"
    }
  },
  {
    "path": "js/16df9ef05001a1741857bf99f5a5738f.js",
    "context": {
      "path": "js/16df9ef05001a1741857bf99f5a5738f.js"
    }
  },
  {
    "path": "js/2a85c11e395a8380b5915443e926b569.js",
    "context": {
      "path": "js/2a85c11e395a8380b5915443e926b569.js"
    }
  },
  {
    "path": "js/34be5330971fdbd18985525bd994b0aa.js",
    "context": {
      "path": "js/34be5330971fdbd18985525bd994b0aa.js"
    }
  },
  {
    "path": "js/35c5f9e096d4da33d2a62031daf14248.js",
    "context": {
      "path": "js/35c5f9e096d4da33d2a62031daf14248.js"
    }
  },
  {
    "path": "js/3d70953a848219e749fedc2cdb906675.js",
    "context": {
      "path": "js/3d70953a848219e749fedc2cdb906675.js"
    }
  },
  {
    "path": "js/3e940a33e44b65c1c0af8bb80a893530.js",
    "context": {
      "path": "js/3e940a33e44b65c1c0af8bb80a893530.js"
    }
  },
  {
    "path": "js/544d012df7acf9c3f0920f67c9e322b9.js",
    "context": {
      "path": "js/544d012df7acf9c3f0920f67c9e322b9.js"
    }
  },
  {
    "path": "js/57d119d998d518b01f9d5ccb5e4d4c52.js",
    "context": {
      "path": "js/57d119d998d518b01f9d5ccb5e4d4c52.js"
    }
  },
  {
    "path": "js/67f6e2f99c3c3133e0dc669919fff5c5.js",
    "context": {
      "path": "js/67f6e2f99c3c3133e0dc669919fff5c5.js"
    }
  },
  {
    "path": "js/7045b35c5bd0e9c7cf59f1900eeeec41.js",
    "context": {
      "path": "js/7045b35c5bd0e9c7cf59f1900eeeec41.js"
    }
  },
  {
    "path": "js/7260bab328b0ad74815a5efb377bcc67.js",
    "context": {
      "path": "js/7260bab328b0ad74815a5efb377bcc67.js"
    }
  },
  {
    "path": "js/893de96f1b6da546bd7c814964723eca.js",
    "context": {
      "path": "js/893de96f1b6da546bd7c814964723eca.js"
    }
  },
  {
    "path": "js/93e29fe348ddc9b71aba9c842adc18b8.js",
    "context": {
      "path": "js/93e29fe348ddc9b71aba9c842adc18b8.js"
    }
  },
  {
    "path": "js/9455859483e31e4da0e28f10d0742c2a.js",
    "context": {
      "path": "js/9455859483e31e4da0e28f10d0742c2a.js"
    }
  },
  {
    "path": "js/9db10375d298678e53777a2347b87073.js",
    "context": {
      "path": "js/9db10375d298678e53777a2347b87073.js"
    }
  },
  {
    "path": "js/9f9b6e54f82a6bbc8bac9b89327024bc.js",
    "context": {
      "path": "js/9f9b6e54f82a6bbc8bac9b89327024bc.js"
    }
  },
  {
    "path": "js/a2261649751fa61b606222c9b2ea3b80.js",
    "context": {
      "path": "js/a2261649751fa61b606222c9b2ea3b80.js"
    }
  },
  {
    "path": "js/b0bade6d42c2702ca85774296cc507c4.js",
    "context": {
      "path": "js/b0bade6d42c2702ca85774296cc507c4.js"
    }
  },
  {
    "path": "js/cd1ed86c1e7f06d985fd71bc10bd4b04.js",
    "context": {
      "path": "js/cd1ed86c1e7f06d985fd71bc10bd4b04.js"
    }
  },
  {
    "path": "js/cecb447a04bbe3e8982190dd6e697120.js",
    "context": {
      "path": "js/cecb447a04bbe3e8982190dd6e697120.js"
    }
  },
  {
    "path": "js/d80b370d82680fc786dcc943a327b9f2.js",
    "context": {
      "path": "js/d80b370d82680fc786dcc943a327b9f2.js"
    }
  },
  {
    "path": "js/df80c5cbcb312a9c7c0b2ebb6ac5f592.js",
    "context": {
      "path": "js/df80c5cbcb312a9c7c0b2ebb6ac5f592.js"
    }
  },
  {
    "path": "js/f1e5dbc1ece900d164c2e9aa2d6a1386.js",
    "context": {
      "path": "js/f1e5dbc1ece900d164c2e9aa2d6a1386.js"
    }
  },
  {
    "path": "js/f3f02c438592c8e1bbe551f4dbbf4f5c.js",
    "context": {
      "path": "js/f3f02c438592c8e1bbe551f4dbbf4f5c.js"
    }
  },
  {
    "path": "our-team.html",
    "context": {
      "title": "Gleeserve Technology Private Limited",
      "first_heading": "OUR TEAM"
    }
  },
  {
    "path": "robotic-process-automation.html",
    "context": {
      "title": "Gleeserve Technology Private Limited",
      "first_heading": "ROBOTIC PROCESS AUTOMATION"
    }
  },
  {
    "path": "service-management.html",
    "context": {
      "title": "Gleeserve Technology Private Limited",
      "first_heading": "SERVICE MANAGEMENT"
    }
  },
  {
    "path": "why-gleeserve.html",
    "context": {
      "title": "Gleeserve Technology Private Limited",
      "first_heading": "WHY GLEESERVE?"
    }
  }
]

Return only a JSON object mapping each path to its new basename (same extension). No other text.