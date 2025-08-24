import React from "react";
import fd8e07869dc13738a779e300a0580e1 from "./07fd8e07869dc13738a779e300a0580e-1.png";
import desktop2 from "./desktop-2.png";
import desktop3 from "./desktop-3.png";
import desktop11 from "./desktop-11.svg";
import frame91 from "./frame-9-1.png";
import image from "./image.png";
import wholeBrandNewShirt22 from "./whole-brand-new-shirt-2-2.png";
import wholeBrandNewShirt31 from "./whole-brand-new-shirt-3-1.png";
import wholeBrandNewShirt41 from "./whole-brand-new-shirt-4-1.png";

export const Frame = (): JSX.Element => {
  return (
    <main className="flex flex-col items-start relative">
      <section className="relative self-stretch w-full h-[1024px]">
        <img
          className="relative self-stretch w-full h-[1024px]"
          alt="Desktop hero section"
          src={desktop3}
        />
      </section>

      <section className="relative w-[1440px] h-[1024px]">
        <img
          className="relative w-[1440px] h-[1024px]"
          alt="Desktop brand section"
          src={desktop11}
        />
      </section>

      <section className="relative self-stretch w-full h-[890px]">
        <img
          className="relative self-stretch w-full h-[890px]"
          alt="Desktop product showcase"
          src={desktop2}
        />
      </section>

      <section className="relative self-stretch w-full h-[736px] bg-[#c6c6c2] overflow-hidden">
        <div className="relative w-[1885px] h-[805px] top-[-35px] left-[-223px]">
          <div className="relative w-[1440px] h-[736px] top-[35px] left-[223px]">
            <img
              className="absolute w-[850px] h-[736px] top-0 left-0 aspect-[1.33] object-cover"
              alt="Whole brand new shirt design variant 1"
              src={wholeBrandNewShirt22}
            />

            <img
              className="absolute w-[850px] h-[736px] top-0 left-[590px] aspect-[1.33] object-cover"
              alt="Whole brand new shirt design variant 2"
              src={wholeBrandNewShirt41}
            />

            <img
              className="absolute w-[1073px] h-[736px] top-0 left-[197px] aspect-[1.33] object-cover"
              alt="Whole brand new shirt design variant 3"
              src={wholeBrandNewShirt31}
            />
          </div>
        </div>
      </section>

      <section className="relative w-[1440px] h-[39px] bg-white">
        <img
          className="absolute w-[1440px] h-[39px] top-0 left-0 aspect-[36.9] object-cover"
          alt="Brand frame divider"
          src={image}
        />
      </section>

      <section className="relative self-stretch w-full h-[418px] bg-white">
        <img
          className="absolute w-[1440px] h-[418px] top-0 left-0 aspect-[0.67] object-cover"
          alt="Product collection showcase"
          src={fd8e07869dc13738a779e300a0580e1}
        />
      </section>

      <section className="relative w-[1440px] h-[39px] bg-white">
        <img
          className="absolute w-[1440px] h-[39px] top-0 left-0 aspect-[36.9] object-cover"
          alt="Footer frame divider"
          src={frame91}
        />
      </section>
    </main>
  );
};
