import React from "react";
import image from "./image.svg";
import practise51 from "./practise5-1.png";
import vector1 from "./vector-1.svg";
import vector2 from "./vector-2.svg";
import vector3 from "./vector-3.svg";
import vector4 from "./vector-4.svg";
import vector from "./vector.svg";

const navigationItems = [
  { label: "Home", href: "#home" },
  { label: "About", href: "#about" },
  { label: "Services", href: "#services" },
  { label: "Contact", href: "#contact" },
];

const logoIcons = [
  {
    src: vector,
    alt: "Vector",
    className: "absolute w-1.5 h-2.5 top-3 left-[29px]",
  },
  {
    src: image,
    alt: "Vector",
    className: "absolute w-2 h-2.5 top-3 left-[39px]",
  },
  {
    src: vector3,
    alt: "Vector",
    className: "absolute w-2 h-2.5 top-3 left-[51px]",
  },
  {
    src: vector4,
    alt: "Vector",
    className: "absolute w-2 h-2.5 top-3 left-16",
  },
];

export const Desktop = (): JSX.Element => {
  const handleButtonClick = () => {
    console.log("Button clicked!");
  };

  return (
    <div className="bg-[#170f0a] grid justify-items-center [align-items:start] w-screen">
      <div className="bg-[#170f0a] w-[1440px] h-[1024px]">
        <div className="relative h-[1024px]">
          <img
            className="absolute w-[1347px] h-[512px] top-[512px] left-0"
            alt="Background vector decoration"
            src={vector1}
          />

          <img
            className="absolute w-[579px] h-[346px] top-0 left-[861px]"
            alt="Background vector decoration"
            src={vector2}
          />

          <main className="inline-flex items-center gap-[113px] absolute top-[169px] left-[134px]">
            <section className="flex flex-col w-[398px] items-start gap-[60px] relative">
              <h1 className="relative self-stretch mt-[-1.00px] [font-family:'Inter-Regular',Helvetica] font-normal text-white text-5xl tracking-[0] leading-[normal]">
                Blaze with Pasion
              </h1>

              <button
                className="all-[unset] box-border inline-flex items-center justify-center gap-2.5 px-10 py-2.5 relative flex-[0_0_auto] bg-[#ec6442] rounded-[50px] shadow-[0px_10px_10px_#170f0a] cursor-pointer transition-all duration-200 hover:bg-[#d55a3a] hover:shadow-[0px_12px_12px_#170f0a] focus:outline-2 focus:outline-white focus:outline-offset-2"
                onClick={handleButtonClick}
                type="button"
                aria-label="Click me button"
              >
                <span className="relative w-fit mt-[-1.00px] [font-family:'Inter-Regular',Helvetica] font-normal text-[#2e2b2b] text-5xl tracking-[0] leading-[normal]">
                  click me
                </span>
              </button>
            </section>

            <img
              className="relative w-[662px] h-[686px] aspect-[0.97]"
              alt="Practice illustration showing a character with flame effects"
              src={practise51}
            />
          </main>

          <header className="absolute w-[1440px] h-[72px] top-0 left-0">
            <div className="flex w-[1350px] items-center justify-center gap-[809px] relative top-[19px] left-[45px]">
              <div
                className="relative w-[132px] h-[35px]"
                role="img"
                aria-label="Company logo"
              >
                <div className="relative h-[35px] aspect-[3.77]">
                  {logoIcons.map((icon, index) => (
                    <img
                      key={index}
                      className={icon.className}
                      alt={icon.alt}
                      src={icon.src}
                    />
                  ))}
                </div>
              </div>

              <nav
                className="inline-flex items-center gap-8 relative flex-[0_0_auto]"
                role="navigation"
                aria-label="Main navigation"
              >
                {navigationItems.map((item, index) => (
                  <a
                    key={index}
                    href={item.href}
                    className="relative w-fit mt-[-1.00px] [font-family:'Inter-Regular',Helvetica] font-normal text-white text-lg tracking-[0.15px] leading-6 whitespace-nowrap hover:text-[#ec6442] transition-colors duration-200 focus:outline-2 focus:outline-white focus:outline-offset-2 focus:rounded"
                  >
                    {item.label}
                  </a>
                ))}
              </nav>
            </div>
          </header>
        </div>
      </div>
    </div>
  );
};

