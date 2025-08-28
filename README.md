# React + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend using TypeScript with type-aware lint rules enabled. Check out the [TS template](https://github.com/vitejs/vite/tree/main/packages/create-vite/template-react-ts) for information on how to integrate TypeScript and [`typescript-eslint`](https://typescript-eslint.io) in your project.


E-come Api  

<!-- https://tituvai.github.io/E-comeApi/Product/index.json -->

https://tituvai.github.io/E-comeApi/Product/index.json


(data.product.data)

elecity Api  

<!-- https://tituvai.github.io/bdApiProducts/products/index.json -->

https://tituvai.github.io/bdApiProducts/products/index.json














<!-- slide dots Part Start   -->

<!-- .custom-dots .slick-dots li button{
  position: absolute;
  bottom: 30px;
  left: 0;
  border-radius: 50%;
  background-color: #7d7d7d;
  
  
}
.custom-dots .slick-dots li.slick-active button {
  background-color: red;
  border: 2px solid white;
} -->
<!-- slide dots Part End  -->



<!-- Next Arrows  -->

import React from 'react'
import { LuChevronRight } from "react-icons/lu";

const NextArrow = (props) => {
    const { onClick } = props;
  return (
      <LuChevronRight className='text-5xl text-deleteC cursor-pointer absolute top-1/2 -right-7 -translate-y-1/2 z-10' onClick={onClick}/>
  )
}

export default NextArrow



<!-- Product Part Api  -->

    const [myproject, setMyProject] = useState ([])

    useEffect (()=>{
        async function AllProduct (){
            let data = await axios.get('https://dummyjson.com/products');
            setMyProject(data.data.products)         
    }
        AllProduct()
    })


    <!-- return -->
    
    {myproject.map(item=>(
                <div className="px-2">
                    <Link to={'/'}><Product productSrc={item.thumbnail} productTitle={item.title} ProductPrice={item.price}/></Link>
                </div>
            ))}



<!-- Add To Card  -->


Uomo  Uomo Uomo 

            <Hadding className={'text-[35px] text-center lg:text-left text-menuC font-bold py-10'} text={'CART'} as={'h3'}/>

            <div className=" lg:pb-20 pb-10 text-center lg:text-left">
            <Hadding className={'text-lg text-menuC font-medium'} text={'SHOPPING BAG'} as={'h6'}/>
            <Peragrap className={'text-deleteC'} peraText={'Manage Your Items List'}/>
            </div>

            {/* Add To cart Part ##################################### */}
            <div className="lg:flex justify-between pb-30">
                <div className="overflow-x-scroll lg:overflow-x-auto">
                    <div className="w-[900px]">
                 <Flex className={'pb-3  border-b-2 border-categoriC'}>
                    <Hadding className={'w-[350px] text-base text-menuC font-medium leading-6'} text={'PRODUCT'} as={'h4'}/>
                    <Hadding className={'w-[150px] text-base text-menuC font-medium leading-6'} text={'PRICE'} as={'h4'}/>
                    <Hadding className={'w-[200px] text-base text-menuC font-medium leading-6'} text={'QUANTITY'} as={'h4'}/>
                    <Hadding className={'w-[200px] text-base text-menuC font-medium leading-6'} text={'SUBTOTAL'} as={'h4'}/>
                </Flex>
                <Flex className={'border-b-2 border-categoriC py-5'}>
                    <div className="w-[350px] flex items-center gap-x-4">
                        <Image imgSrc={cart} imgAlt={'cart.png'}/>
                        <div className="">
                        <Hadding className={'text-base text-menuC font-medium'} text={'Zessi Dresses'} as={'h6'}/>
                        <Hadding className={'text-base text-deleteC'} text={'yellow'} as={'h6'}/>
                        <Hadding className={'text-base text-deleteC'} text={'xl'} as={'h6'}/>
                        </div>
                    </div>
                    <div className="w-[150px]">
                        <Hadding className={'text-base text-deleteC font-medium'} text={'$99'} as={'h5'}/>
                    </div>
                    <div className="w-[200px]">
                        <div className="lg:w-[120px] w-[80px] p-1 lg:p-3 border-2 border-categoriC flex items-center justify-between">
                            <span className='text-2xl text-deleteC font-medium'>-</span>
                            <span className='text-base text-deleteC font-medium'>3</span>
                            <span className='text-base text-deleteC font-medium'>+</span>
                        </div>
                    </div>
                    <div className="w-[150px]">
                        <Hadding className={'text-base text-menuC font-medium'} text={'$399'} as={'h4'}/>
                    </div>
                    <div className="w-[50px]">
                       <MdOutlineClear className='text-lg text-deleteC'/> 
                    </div>
                </Flex>
                <Flex className={'border-b-2 border-categoriC py-5'}>
                    <div className="w-[350px] flex items-center gap-x-4">
                        <Image imgSrc={cartOne} imgAlt={'cart1.png'}/>
                        <div className="">
                        <Hadding className={'text-base text-menuC font-medium'} text={'Kirby T-Shirt'} as={'h6'}/>
                        <Hadding className={'text-base text-deleteC'} text={'black'} as={'h6'}/>
                        <Hadding className={'text-base text-deleteC'} text={'m'} as={'h6'}/>
                        </div>
                    </div>
                    <div className="w-[150px]">
                        <Hadding className={'text-base text-deleteC font-medium'} text={'$79'} as={'h5'}/>
                    </div>
                    <div className="w-[200px]">
                        <div className="lg:w-[120px] w-[80px] p-1 lg:p-3 border-2 border-categoriC flex items-center justify-between">
                            <span className='text-2xl text-deleteC font-medium'>-</span>
                            <span className='text-base text-deleteC font-medium'>4</span>
                            <span className='text-base text-deleteC font-medium'>+</span>
                        </div>
                    </div>
                    <div className="w-[150px]">
                        <Hadding className={'text-base text-menuC font-medium'} text={'$279'} as={'h4'}/>
                    </div>
                    <div className="w-[50px]">
                       <MdOutlineClear className='text-lg text-deleteC'/> 
                    </div>
                </Flex>
                <Flex className={'border-b-2 border-categoriC py-5'}>
                    <div className="w-[350px] flex items-center gap-x-4">
                        <Image imgSrc={cartTwo} imgAlt={'cart2.png'}/>
                        <div className="">
                        <Hadding className={'text-base text-menuC font-medium'} text={'Cableknit Shawl'} as={'h6'}/>
                        <Hadding className={'text-base text-deleteC'} text={'red'} as={'h6'}/>
                        <Hadding className={'text-base text-deleteC'} text={'xxl'} as={'h6'}/>
                        </div>
                    </div>
                    <div className="w-[150px]">
                        <Hadding className={'text-base text-deleteC font-medium'} text={'$87'} as={'h5'}/>
                    </div>
                    <div className="w-[200px]">
                        <div className="lg:w-[120px] w-[80px] p-1 lg:p-3 border-2 border-categoriC flex items-center justify-between">
                            <span className='text-2xl text-deleteC font-medium'>-</span>
                            <span className='text-base text-deleteC font-medium'>3</span>
                            <span className='text-base text-deleteC font-medium'>+</span>
                        </div>
                    </div>
                    <div className="w-[150px]">
                        <Hadding className={'text-base text-menuC font-medium'} text={'$268'} as={'h4'}/>
                    </div>
                    <div className="w-[50px]">
                       <MdOutlineClear className='text-lg text-deleteC'/> 
                    </div>
                </Flex>
                <Flex className={'py-10 px-3 lg:px-0'}>
                    <div className="w-[300px]  lg:w-[400px] relative border border-categoriC">
                        <input className=' p-4 placeholder:text-base placeholder:text-deleteC outline-0 ' type="text" placeholder='Coupon Code' />
                        <span className='text-base text-menuC font-medium absolute right-5 top-1/2 -translate-y-1/2 cursor-pointer'>APPLY COUPON</span>
                    </div>
                    <div className="">
                        <button className='text-base text-menuC px-7 py-4 bg-footerBg cursor-pointer'>UPDATE CART</button>
                    </div>
                </Flex>
                </div>
            </div>